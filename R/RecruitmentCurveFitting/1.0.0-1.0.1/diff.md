# Comparing `tmp/RecruitmentCurveFitting-1.0.0-py2.py3-none-any.whl.zip` & `tmp/RecruitmentCurveFitting-1.0.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 105224 bytes, number of entries: 12
+Zip file size: 105806 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    35821 b- defN 23-May-27 05:45 RecruitmentCurveFitting/COPYING
--rw-r--r--  2.0 unx    18139 b- defN 23-May-27 05:02 RecruitmentCurveFitting/CurveFitting.py
+-rw-r--r--  2.0 unx    18188 b- defN 23-May-27 23:59 RecruitmentCurveFitting/CurveFitting.py
 -rw-r--r--  2.0 unx    28108 b- defN 23-May-27 05:02 RecruitmentCurveFitting/RecruitmentCurves.py
--rw-r--r--  2.0 unx     3967 b- defN 23-May-27 05:21 RecruitmentCurveFitting/__init__.py
--rw-r--r--  2.0 unx     6445 b- defN 23-May-27 05:01 RecruitmentCurveFitting/__main__.py
+-rw-r--r--  2.0 unx     4153 b- defN 23-May-27 23:59 RecruitmentCurveFitting/__init__.py
+-rw-r--r--  2.0 unx     6695 b- defN 23-May-27 23:59 RecruitmentCurveFitting/__main__.py
 -rw-r--r--  2.0 unx     1491 b- defN 23-May-27 02:43 RecruitmentCurveFitting/example-data1.txt
 -rw-r--r--  2.0 unx     2291 b- defN 23-May-27 02:24 RecruitmentCurveFitting/example-data2.txt
 -rw-r--r--  2.0 unx   208425 b- defN 23-May-27 02:24 RecruitmentCurveFitting/example-waveforms.csv
--rw-r--r--  2.0 unx     1545 b- defN 23-May-27 05:46 RecruitmentCurveFitting-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-27 05:46 RecruitmentCurveFitting-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-May-27 05:46 RecruitmentCurveFitting-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1135 b- defN 23-May-27 05:46 RecruitmentCurveFitting-1.0.0.dist-info/RECORD
-12 files, 307501 bytes uncompressed, 103284 bytes compressed:  66.4%
+-rw-r--r--  2.0 unx     2602 b- defN 23-May-27 23:59 RecruitmentCurveFitting-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-27 23:59 RecruitmentCurveFitting-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-May-27 23:59 RecruitmentCurveFitting-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1135 b- defN 23-May-27 23:59 RecruitmentCurveFitting-1.0.1.dist-info/RECORD
+12 files, 309043 bytes uncompressed, 103866 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: RecruitmentCurveFitting/example-data2.txt
 Comment: 
 
 Filename: RecruitmentCurveFitting/example-waveforms.csv
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.0.0.dist-info/METADATA
+Filename: RecruitmentCurveFitting-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.0.0.dist-info/WHEEL
+Filename: RecruitmentCurveFitting-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.0.0.dist-info/top_level.txt
+Filename: RecruitmentCurveFitting-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.0.0.dist-info/RECORD
+Filename: RecruitmentCurveFitting-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## RecruitmentCurveFitting/CurveFitting.py

```diff
@@ -133,14 +133,15 @@
 	    # And now re-do the fit with a fixed offset
 	    z.c.fixedValue = 1.5
 	    z.Fit().Plot( data=False, hold=True, label=str(z.pdict) )
 	    from matplotlib.pyplot import legend; legend()
 	"""
 
 	_PARAMS = []
+	__hooks = []
 	def __init__( self, x, y=(), robust=False, fix=None, excuses=None, **descriptors ):
 		"""
 		Args:
 		    robust (bool):
 		        set the default mode for `.Fit()`:  soft-L1 loss if `True`,
 		        L2 loss otherwise.
 		    
@@ -153,14 +154,15 @@
 		        non-empty, curve-fitting will be skipped for this dataset.
 		    
 		    **descriptors:
 		        any further keyword arguments are stored in the
 		        `self.descriptors` dictionary to distinguish this dataset
 		        from other datasets (experimental conditions, etc).
 		"""
+		for hook in self.__hooks: hook()
 		if isinstance( x, Curve ):
 			other = x
 			self._PARAMS = copy.deepcopy( other._PARAMS ) # includes information from `fix`
 			self.fittingException = other.fittingException
 			self.x = other.x.copy()
 			self.y = other.y.copy()
 			self.robust = other.robust
```

## RecruitmentCurveFitting/__init__.py

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
 
+__version__ = '1.0.1'
+
 # $BEGIN_RECRUITMENTCURVEFITTING_LICENSE$
 # 
 # This file is part of the RecruitmentCurveFitting project, a Python
 # package for fitting sigmoid and bell-shaped functions to EMG
 # recruitment-curve measurements.
 # 
 # Copyright (c) 2023 Jeremy Hill
@@ -26,80 +28,81 @@
 __all__ = [ 'Cite' ]
 import os, sys, ast
 from . import RecruitmentCurves
 __doc__ = RecruitmentCurves.__doc__
 __all__ += RecruitmentCurves.__all__
 from .RecruitmentCurves import *
 
-__version__ = '1.0.0'
-
 CITATION_INFO = """
-If you use this software in your research, your report should cite
-the article in which this approach was introduced, as follows:
+If you use this software in your research, your report should cite the article
+in which this approach was introduced, as follows:
 
 - McKinnon ML, Hill NJ, Carp JS, Dellenbach B & Thompson AK (2023).
-  Automated identification of EMG responses evoked by peripheral
-  nerve stimulation: quantitative effects on critical parameters
-  of diagnostic and closed-loop therapeutic applications.
+  Automated identification of EMG responses evoked by peripheral nerve
+  stimulation: quantitative effects on critical parameters of diagnostic and
+  closed-loop therapeutic applications.
   @JOURNAL@ @NUMBER@(@VOLUME@):@PAGES@
   @DOI@
     
 The corresponding BibTeX entry is::
 
     @article{mckinnonhill2023,
-        author  = {McKinnon, Michael L. and Hill, N. Jeremy  and  Carp, Jonathan S.  and Dellenbach, Blair and Thompson, Aiko K.},
-        title   = {Automated Identification of {EMG} Responses Evoked by Peripheral Nerve Stimulation: Quantitative Effects on Critical Parameters of Diagnostic and Closed-Loop Therapeutic Applications},
-        journal = {xxxx},
-        volume  = {x},
-        number  = {x},
-        pages   = {xx-xx},
-        month   = {xxx},
-        year    = {2023},
-        date    = {2023-xx-xx},
-        doi     = {xxx/xxxx},
-        url     = {https://doi.org/xxx/xxxx},
+      author  = {McKinnon, Michael L. and Hill, N. Jeremy and Carp, Jonathan S.
+                 and Dellenbach, Blair and Thompson, Aiko K.},
+      title   = {Automated Identification of {EMG} Responses Evoked by Peripheral
+                 Nerve Stimulation: Quantitative Effects on Critical Parameters 
+                 of Diagnostic and Closed-Loop Therapeutic Applications},
+      journal = {TBD},
+      volume  = {TBD},
+      number  = {TBD},
+      pages   = {TBD--TBD},
+      month   = {TBD},
+      year    = {2023},
+      date    = {2023-TBD-TBD},
+      doi     = {TBD/TBD},
+      url     = {https://doi.org/TBD/TBD},
     }
 """
 
 def Cite( command=None, prefix='', stream=None ):
 	"""
-=============================================================
-This is the RecruitmentCurveFitting package version @VERSION@
-by Jeremy Hill, running in Python @PYVERSION@.
+=============================================================================
+This is the RecruitmentCurveFitting package version @VERSION@ by Jeremy Hill,
+running in Python @PYVERSION@.
 
 @CITATION_INFO@
 
-To acknowledge this message and prevent it from being displayed
-every time you import the package::
+To acknowledge this message and prevent it from being displayed every time you
+start using the package::
 
 	from RecruitmentCurveFitting import Cite
 	Cite('agree')
 
 To refer back to this information again, simply call `Cite()`.
-=============================================================
+=============================================================================
 	"""
 	if isinstance( command, str ):
 		command = command.lower()
-		if command in [ 'on_import' ]:
-			if not Preferences().get( 'silent', False ):
-				command = None
-		elif command in [ 'agree', 'acknowledge', 'ok' ]:
-			Preferences( silent=True )
-		else:
-			raise ValueError( 'unrecognized command option' )
+		if command in [ 'agree', 'acknowledge', 'ok' ]: Preferences( nag=False )
+		else: raise ValueError( 'unrecognized command option' )
 	if command is None:
 		if stream is None: stream = sys.stdout
 		stream.write( '\n'.join( prefix + line for line in Cite.__doc__.split( '\n' ) ) + '\n' )
 		try: stream.flush()
 		except: pass
+Cite.__doc__ = Cite.__doc__.replace( '@VERSION@', __version__ ).replace( '@PYVERSION@', '%s.%s' % ( sys.version_info.major, sys.version_info.minor ) ).replace( '@CITATION_INFO@', CITATION_INFO.strip() )
+hooks = [ lambda: ( 
+	( Preferences().get( 'nag', True ) and Cite( stream=sys.stderr, prefix='# ' ) ),
+	hooks.pop( 0 )
+) ]
+#from . import CurveFitting; CurveFitting.Curve._Curve__hooks = hooks
+# TODO: uncomment the line above when the citation info is finalized, to arm the nag message
 def Preferences( **kwargs ):
-	prefsFile = os.path.expanduser( '~/.RecruitmentCurveFitting' )
+	prefsFile = os.path.expanduser( '~/.' + __name__ )
 	try: prefs = ast.literal_eval( open( prefsFile, 'rt' ).read() )
 	except: prefs = {}
 	if kwargs:
 		prefs.update( kwargs )
 		prefsText = '{\n' + ''.join( '\t%r : %r,\n' % item for item in prefs.items() ) + '}\n'
 		prefs = ast.literal_eval( prefsText )
 		open( prefsFile, 'wt' ).write( prefsText )
 	return prefs
-Cite.__doc__ = Cite.__doc__.rstrip().replace( '@VERSION@', __version__ ).replace( '@PYVERSION@', '%s.%s' % ( sys.version_info.major, sys.version_info.minor ) ).replace( '@CITATION_INFO@', CITATION_INFO.strip() )
-Cite( 'on_import', stream=sys.stderr )
```

## RecruitmentCurveFitting/__main__.py

```diff
@@ -25,39 +25,47 @@
 # $END_RECRUITMENTCURVEFITTING_LICENSE$
 
 """
 Use the RecruitmentCurveFitting module from the command-line
 to fit both an M-wave and an H-reflex recruitment curve from
 one or more text files.
 """
-from RecruitmentCurveFitting import *
 
 import argparse
 class HelpFormatter( argparse.RawDescriptionHelpFormatter ): pass
 #class HelpFormatter( argparse.RawDescriptionHelpFormatter, argparse.ArgumentDefaultsHelpFormatter ): pass
 parser = argparse.ArgumentParser( description=__doc__, formatter_class=HelpFormatter, prog='python -m RecruitmentCurveFitting', )
 parser.add_argument(         "filenames",    metavar='FILENAME',    nargs='*', help='one or more text files to load (use a dash to denote stdin)' )
 parser.add_argument( "-t", "--threshold",    metavar='MTHRESHOLD',  default=0.1, type=float, help='unscaled proportion of Mmax (between 0 and 1) that is considered "threshold" for the M-wave curve' )
 parser.add_argument( "-s", "--saveas",       metavar='PDFFILENAME', default='', help='name of pdf file in which to save figures' )
 parser.add_argument( "-p", "--plot",         action='store_true',   help='whether to show figures on-screen' )
 parser.add_argument( "-g", "--grid",         action='store_true',   help='whether to use a grid for the plot' )
 parser.add_argument( "-x", "--xlabel",       metavar='XLABEL',      default='Stimulation Intensity (mA)', help='x-axis label text for the plot' )
 parser.add_argument( "-y", "--ylabel",       metavar='YLABEL',      default='Response ($\\mu$V)', help='y-axis label text for the plot' )
 parser.add_argument(       "--unpack-examples", action='store_true', help='write example files to the current directory (do not overwrite) and quit' )
+parser.add_argument(       "--help-module",  action='store_true', help='display the main package docstring' )
 opts = parser.parse_args()
 
 import os, re, ast, sys, glob
 import numpy
-def tryeval(x):
-	try: return ast.literal_eval( x )
-	except: return x
-	
+
+import RecruitmentCurveFitting
+from RecruitmentCurveFitting import *
+
 if opts.unpack_examples:
 	UnpackExamples()
 	if not opts.filenames: raise SystemExit( 'done' )		
+
+if opts.help_module:
+	print( RecruitmentCurveFitting.__doc__ )
+	if not opts.filenames: raise SystemExit()
+
+def tryeval(x):
+	try: return ast.literal_eval( x )
+	except: return x
 	
 filenames = opts.filenames if opts.filenames else [ '-' ]
 def myglob( pattern ):
 	hits = sorted( glob.glob( os.path.expanduser( pattern ) ) )
 	return hits if hits else [ pattern ]
 filenames = [ filename for pattern in filenames for filename in myglob( pattern ) ]
 conditions = {}
@@ -92,14 +100,15 @@
 conditionIndex = numpy.array( [ conditions.setdefault( conditionRow, len( conditions ) + 1 ) for conditionRow in collatedConditionTable ] )
 conditions = { v : dict( k ) for k, v in conditions.items() }
 collatedDataTable = numpy.concatenate( collatedDataTable, axis=0 )
 stim       = collatedDataTable[ :, -3 ]
 mResponse  = collatedDataTable[ :, -2 ]
 hResponse  = collatedDataTable[ :, -1 ]
 if opts.plot and 'IPython' in sys.modules: import matplotlib; matplotlib.interactive( True )
+
 print( '[' )
 for eachCondition, conditionDict in conditions.items():
 	selected = conditionIndex == eachCondition
 	m = Sigmoid(   stim[ selected ], mResponse[ selected ], **conditionDict )
 	h = HillCurve( stim[ selected ], hResponse[ selected ], **conditionDict ) # TODO: add option for ModifiedBrinkworth
 	mMax = m.uHeight.finalValue
 	mThresholdStim = m.Backward( opts.threshold, scaled=False ) if opts.threshold is not None and 0 < opts.threshold < 1 else None
```

## Comparing `RecruitmentCurveFitting-1.0.0.dist-info/RECORD` & `RecruitmentCurveFitting-1.0.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 RecruitmentCurveFitting/COPYING,sha256=Czg9WmPaZE9ijZnDOXbqZIftiaqlnwsyV5kt6sEXHms,35821
-RecruitmentCurveFitting/CurveFitting.py,sha256=pMdEpMVbJ0jEFJsDh_WAyqZsy7-RcS5k2F1cyq3_Aq4,18139
+RecruitmentCurveFitting/CurveFitting.py,sha256=2QrG4bXN-4TIZiNEQcW1U3EQbXxuhMC2620CBUzZbFE,18188
 RecruitmentCurveFitting/RecruitmentCurves.py,sha256=Glpy6G3ttJ1gBnIv0ITVPr4MtSTLslWauWRZbqOFK8g,28108
-RecruitmentCurveFitting/__init__.py,sha256=uE9O6aow7BO3aaXvQs5FsIewyiRZzw04j6ejkki722g,3967
-RecruitmentCurveFitting/__main__.py,sha256=EGaNutByQZaNBb2PxU20K_i4ikhwOWJN-I6lvDPD7aE,6445
+RecruitmentCurveFitting/__init__.py,sha256=ZiUIZ1Vn1r9p0Fm7jooQ3T8a89xWdAVd4Dav6iUFnUU,4153
+RecruitmentCurveFitting/__main__.py,sha256=I71DOcLNvMHohrnGZQjaMPLSD9zdiFRqikEvV3JUCpI,6695
 RecruitmentCurveFitting/example-data1.txt,sha256=FeaYwnAMGemLQKM9Kj1IPi_3fey7gyY9SLOJYttZcXc,1491
 RecruitmentCurveFitting/example-data2.txt,sha256=SBv6zHDxt1YOhylfZSMMHSCsDNwL1brHpTgAdH8esvg,2291
 RecruitmentCurveFitting/example-waveforms.csv,sha256=eWF7HtChJAv5uHfiQ1Pg__l-d9eYKtGWr8PlYp7-kis,208425
-RecruitmentCurveFitting-1.0.0.dist-info/METADATA,sha256=kNc6efoHiOc5rAX6uqFgYg5GE0PKphC9Z_Hsa3cp57k,1545
-RecruitmentCurveFitting-1.0.0.dist-info/WHEEL,sha256=h_aVn5OB2IERUjMbi2pucmR_zzWJtk303YXvhh60NJ8,110
-RecruitmentCurveFitting-1.0.0.dist-info/top_level.txt,sha256=GaYHShtnr9zJ_unau13fDnezLMr3kyCH0-KQN_Go6WM,24
-RecruitmentCurveFitting-1.0.0.dist-info/RECORD,,
+RecruitmentCurveFitting-1.0.1.dist-info/METADATA,sha256=Kpsp9DWWQv1EU5TA8jB3_trvq_L46nZQ5kXS-iTIW1s,2602
+RecruitmentCurveFitting-1.0.1.dist-info/WHEEL,sha256=h_aVn5OB2IERUjMbi2pucmR_zzWJtk303YXvhh60NJ8,110
+RecruitmentCurveFitting-1.0.1.dist-info/top_level.txt,sha256=GaYHShtnr9zJ_unau13fDnezLMr3kyCH0-KQN_Go6WM,24
+RecruitmentCurveFitting-1.0.1.dist-info/RECORD,,
```


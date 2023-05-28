# Comparing `tmp/META_TOOLBOX-2023.1.tar.gz` & `tmp/META_TOOLBOX-2023.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "META_TOOLBOX-2023.1.tar", last modified: Sat Feb 11 12:36:00 2023, max compression
+gzip compressed data, was "META_TOOLBOX-2023.2.tar", last modified: Sun May 28 01:14:31 2023, max compression
```

## Comparing `META_TOOLBOX-2023.1.tar` & `META_TOOLBOX-2023.2.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-02-11 12:36:00.478340 META_TOOLBOX-2023.1/
-drwxrwxrwx   0        0        0        0 2023-02-11 12:36:00.462338 META_TOOLBOX-2023.1/META_TOOLBOX/
--rw-rw-rw-   0        0        0    29288 2023-02-10 22:40:06.000000 META_TOOLBOX-2023.1/META_TOOLBOX/META.py
--rw-rw-rw-   0        0        0     8119 2023-02-02 11:00:48.000000 META_TOOLBOX-2023.1/META_TOOLBOX/META_CO_LIBRARY.py
--rw-rw-rw-   0        0        0     9421 2022-11-15 00:21:19.000000 META_TOOLBOX-2023.1/META_TOOLBOX/META_FA_LIBRARY.py
--rw-rw-rw-   0        0        0     6654 2023-01-30 18:22:05.000000 META_TOOLBOX-2023.1/META_TOOLBOX/META_FUNCTIONS.py
--rw-rw-rw-   0        0        0    20066 2022-12-13 17:41:35.000000 META_TOOLBOX-2023.1/META_TOOLBOX/META_GRAPHICS_LIBRARY.py
--rw-rw-rw-   0        0        0      958 2023-02-10 22:40:06.000000 META_TOOLBOX-2023.1/META_TOOLBOX/META_HC_LIBRARY.py
--rw-rw-rw-   0        0        0     2647 2023-02-10 22:40:06.000000 META_TOOLBOX-2023.1/META_TOOLBOX/META_SA_LIBRARY.py
--rw-rw-rw-   0        0        0      216 2023-01-30 18:20:16.000000 META_TOOLBOX-2023.1/META_TOOLBOX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-11 12:36:00.476341 META_TOOLBOX-2023.1/META_TOOLBOX.egg-info/
--rw-rw-rw-   0        0        0      642 2023-02-11 12:36:00.000000 META_TOOLBOX-2023.1/META_TOOLBOX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-02-11 12:36:00.000000 META_TOOLBOX-2023.1/META_TOOLBOX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-11 12:36:00.000000 META_TOOLBOX-2023.1/META_TOOLBOX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-02-11 12:36:00.000000 META_TOOLBOX-2023.1/META_TOOLBOX.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-11 12:36:00.000000 META_TOOLBOX-2023.1/META_TOOLBOX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      642 2023-02-11 12:36:00.477339 META_TOOLBOX-2023.1/PKG-INFO
--rw-rw-rw-   0        0        0      626 2022-10-28 01:32:06.000000 META_TOOLBOX-2023.1/README.md
--rw-rw-rw-   0        0        0       42 2023-02-11 12:36:00.478340 META_TOOLBOX-2023.1/setup.cfg
--rw-rw-rw-   0        0        0      730 2023-02-11 12:35:53.000000 META_TOOLBOX-2023.1/setup.py
+drwxrwxr-x   0 wanderlei  (1000) wanderlei  (1000)        0 2023-05-28 01:14:31.053979 META_TOOLBOX-2023.2/
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)    11357 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/LICENSE
+drwxrwxr-x   0 wanderlei  (1000) wanderlei  (1000)        0 2023-05-28 01:14:31.053979 META_TOOLBOX-2023.2/META_TOOLBOX/
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)    38741 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     7901 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_CO_LIBRARY.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      112 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_DE_LIBRARY.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)    14095 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_FA_LIBRARY.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     6332 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_FUNCTIONS.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     1410 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_GA_LIBRARY.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)    19743 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_GRAPHICS_LIBRARY.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      929 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_HC_LIBRARY.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     3650 2023-05-28 00:47:17.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_KNAPSACK.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     1280 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_PSO_LIBRARY.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     2544 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/META_TOOLBOX/META_SA_LIBRARY.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      333 2023-05-27 23:50:52.000000 META_TOOLBOX-2023.2/META_TOOLBOX/__init__.py
+drwxrwxr-x   0 wanderlei  (1000) wanderlei  (1000)        0 2023-05-28 01:14:31.053979 META_TOOLBOX-2023.2/META_TOOLBOX.egg-info/
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      624 2023-05-28 01:14:31.000000 META_TOOLBOX-2023.2/META_TOOLBOX.egg-info/PKG-INFO
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      575 2023-05-28 01:14:31.000000 META_TOOLBOX-2023.2/META_TOOLBOX.egg-info/SOURCES.txt
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)        1 2023-05-28 01:14:31.000000 META_TOOLBOX-2023.2/META_TOOLBOX.egg-info/dependency_links.txt
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)       24 2023-05-28 01:14:31.000000 META_TOOLBOX-2023.2/META_TOOLBOX.egg-info/requires.txt
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)       13 2023-05-28 01:14:31.000000 META_TOOLBOX-2023.2/META_TOOLBOX.egg-info/top_level.txt
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      624 2023-05-28 01:14:31.053979 META_TOOLBOX-2023.2/PKG-INFO
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      607 2023-05-27 23:22:01.000000 META_TOOLBOX-2023.2/README.md
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)       38 2023-05-28 01:14:31.053979 META_TOOLBOX-2023.2/setup.cfg
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      730 2023-05-28 01:00:12.000000 META_TOOLBOX-2023.2/setup.py
```

### Comparing `META_TOOLBOX-2023.1/META_TOOLBOX/META.py` & `META_TOOLBOX-2023.2/META_TOOLBOX/META.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,654 +1,873 @@
-import numpy as np
-import time
-import META_TOOLBOX.META_CO_LIBRARY as META_CO
-import META_TOOLBOX.META_HC_LIBRARY as META_HC
-import META_TOOLBOX.META_SA_LIBRARY as META_SA
-import META_TOOLBOX.META_FA_LIBRARY as META_FA
-from datetime import datetime
-
-def HELLO():
-    """
-    Test function.
-    """
-    print("hello world")
-    return
-
-def HILL_CLIMBING_001(OF_FUNCTION, SETUP):
-    """ 
-    Standard Hill climbing algorithm. Continuous version. The algorithm also presents the results formatted in a spreadsheet.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/HC.html
-    """
-    
-    # Setup config
-    N_REP = SETUP['N_REP']
-    N_ITER = SETUP['N_ITER']
-    N_POP = SETUP['N_POP']
-    D = SETUP['D']
-    X_L = SETUP['X_L']
-    X_U = SETUP['X_U']
-    NULL_DIC = SETUP['NULL_DIC']
-    MODEL_NAME = 'META_HC001_'
-
-    # Parameters
-    PARAMETERS = SETUP['PARAMETERS']
-    SIGMA = (PARAMETERS['SIGMA'] / 100)
-    
-    # Creating variables in the repetitions procedure
-    RESULTS_REP = []
-    BEST_REP = []
-    WORST_REP = []
-    AVERAGE_REP = []
-    NAME = []
-    if NULL_DIC == None:
-        NULL_DIC = []
-    else:
-        pass 
-    
-    # Repetition looping
-    INIT = time.time()
-    for REP in range(N_REP):
-        
-        # Creating variables in the iterations procedure
-        OF = np.zeros((N_POP, 1)); 
-        FIT = np.zeros((N_POP, 1))
-        RESULTS_ITER = [{'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': J} for J in range(N_POP)]
-        BEST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
-        AVERAGE_ITER = {'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1)}
-        WORST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
-        NEOF_COUNT = 0 
-        
-        # Initial population
-        X = META_CO.INITIAL_POPULATION_01(N_POP, D, X_L, X_U)
-        for I in range(N_POP):
-            OF[I, 0] = OF_FUNCTION(X[I, :], NULL_DIC)
-            FIT[I, 0] = META_CO.FIT_VALUE(OF[I, 0])
-            NEOF_COUNT += 1
-               
-        # Storage all values in RESULTS_ITER
-        for I, X_ALL, OF_ALL, FIT_ALL, in zip(RESULTS_ITER, X, OF, FIT):
-            I['X_POSITION'][0, :] = X_ALL
-            I['OF'][0] = OF_ALL
-            I['FIT'][0] = FIT_ALL
-            I['PARAMETERS'][0] = None
-            I['NEOF'][0] = NEOF_COUNT
-        
-        # Best, average and worst storage
-        BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
-        BEST_ITER['ID_PARTICLE'][0] = BEST_POSITION
-        WORST_ITER['ID_PARTICLE'][0] = WORST_POSITION
-        BEST_ITER['X_POSITION'][0, :] = X_BEST
-        WORST_ITER['X_POSITION'][0, :] = X_WORST
-        BEST_ITER['OF'][0] = OF_BEST
-        AVERAGE_ITER['OF'][0] = OF_AVERAGE
-        WORST_ITER['OF'][0] = OF_WORST
-        BEST_ITER['FIT'][0] = FIT_BEST
-        AVERAGE_ITER['FIT'][0] = FIT_AVERAGE
-        WORST_ITER['FIT'][0] = FIT_WORST
-        BEST_ITER['PARAMETERS'][0] = None
-        BEST_ITER['NEOF'][0] = NEOF_COUNT
-        AVERAGE_ITER['NEOF'][0] = NEOF_COUNT
-        WORST_ITER['NEOF'][0] = NEOF_COUNT
-        
-        # Iteration procedure
-        for ITER in range(N_ITER):
-
-            # Population movement
-            for POP in range(N_POP):
-                
-                # Hill Climbing particle movement
-                X_ITEMP, OF_ITEMP, FIT_ITEMP, NEOF = META_HC.HC_MOVEMENT(OF_FUNCTION, NULL_DIC, X[POP, :], X_L, X_U, D, SIGMA) 
-                
-                # New design variables
-                if FIT_ITEMP > FIT[POP, 0]:
-                    X[POP, :] = X_ITEMP
-                    OF[POP, 0] = OF_ITEMP
-                    FIT[POP, 0] = FIT_ITEMP
-                else:
-                    pass
-                
-                # Update NEOF (Number of Objective Function Evaluations)
-                NEOF_COUNT += NEOF
-            
-            # Storage all values in RESULTS_ITER
-            for I, X_ALL, OF_ALL, FIT_ALL  in zip(RESULTS_ITER, X, OF, FIT):
-                I['X_POSITION'][ITER + 1, :] = X_ALL
-                I['OF'][ITER + 1] = OF_ALL
-                I['FIT'][ITER + 1] = FIT_ALL
-                I['PARAMETERS'][ITER + 1] = None
-                I['NEOF'][ITER + 1] = NEOF_COUNT
-            
-            # Best, average and worst storage
-            BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
-            BEST_ITER['ID_PARTICLE'][ITER + 1] = BEST_POSITION
-            WORST_ITER['ID_PARTICLE'][ITER + 1] = WORST_POSITION
-            BEST_ITER['X_POSITION'][ITER + 1, :] = X_BEST
-            WORST_ITER['X_POSITION'][ITER + 1, :] = X_WORST
-            BEST_ITER['OF'][ITER + 1] = OF_BEST
-            AVERAGE_ITER['OF'][ITER + 1] = OF_AVERAGE
-            WORST_ITER['OF'][ITER + 1] = OF_WORST
-            BEST_ITER['FIT'][ITER + 1] = FIT_BEST
-            AVERAGE_ITER['FIT'][ITER + 1] = FIT_AVERAGE
-            WORST_ITER['FIT'][ITER + 1] = FIT_WORST
-            BEST_ITER['PARAMETERS'][ITER + 1] = None
-            BEST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
-            AVERAGE_ITER['NEOF'][ITER + 1] = NEOF_COUNT
-            WORST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
-        
-        # Append iteration results
-        RESULTS_REP.append(RESULTS_ITER)
-        BEST_REP.append(BEST_ITER)
-        AVERAGE_REP.append(AVERAGE_ITER)
-        WORST_REP.append(WORST_ITER)
-        
-        # Progress bar update
-        time.sleep(0.01)
-        META_CO.PROGRESS_BAR(REP + 1, N_REP)
-    END = time.time()
-    
-    # Resume process (Time and Excel outputs)
-    print('Process Time: %.2f' % (END - INIT), 'Seconds', '\n', 'Seconds per repetition: %.2f' % ((END - INIT) / N_REP))
-    STATUS_PROCEDURE = META_CO.SUMMARY_ANALYSIS(BEST_REP, N_REP, N_ITER)
-    for REP in range(N_REP):
-        NAME.append(MODEL_NAME + 'REP_' + str(REP) + '_BEST_' + str(REP) + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S')))
-        META_CO.EXCEL_WRITER_ITERATION(NAME[REP], D, BEST_REP[REP])
-    NAME_RESUME = MODEL_NAME + 'RESUME' + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S'))
-    META_CO.EXCEL_PROCESS_RESUME(NAME_RESUME, D, BEST_REP, N_ITER, N_REP)    
-    
-    return RESULTS_REP, BEST_REP, AVERAGE_REP, WORST_REP, STATUS_PROCEDURE
-
-def SIMULATED_ANNEALING_001(OF_FUNCTION, SETUP):
-    """ 
-    Standard Simulated annealing algorithm. Continuous version. The algorithm also presents the results formatted in a spreadsheet.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/SA001.html
-    """
-    
-    # Setup config
-    N_REP = SETUP['N_REP']
-    N_ITER = SETUP['N_ITER']
-    N_POP = SETUP['N_POP']
-    D = SETUP['D']
-    X_L = SETUP['X_L']
-    X_U = SETUP['X_U']
-    NULL_DIC = SETUP['NULL_DIC']
-    MODEL_NAME = 'META_SA001_'
-
-    # Parameters
-    PARAMETERS = SETUP['PARAMETERS']
-    SIGMA = (PARAMETERS['SIGMA'] / 100)
-    SCHEDULE = PARAMETERS['COOLING SCHEME']
-    ALPHA = PARAMETERS['TEMP_FACTOR']
-    TEMP_INI = PARAMETERS['T_0']
-        
-    # Creating variables in the repetitions procedure
-    RESULTS_REP = []
-    BEST_REP = []
-    WORST_REP = []
-    AVERAGE_REP = []
-    NAME = []
-    if NULL_DIC == None:
-        NULL_DIC = []
-    else:
-        pass 
-    
-    # Repetition looping
-    INIT = time.time()
-    for REP in range(N_REP):
-        
-        # Creating variables in the iterations procedure
-        OF = np.zeros((N_POP, 1)); 
-        FIT = np.zeros((N_POP, 1))
-        RESULTS_ITER = [{'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': J} for J in range(N_POP)]
-        BEST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
-        AVERAGE_ITER = {'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1)}
-        WORST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
-        NEOF_COUNT = 0 
-        
-        # Initial population
-        X = META_CO.INITIAL_POPULATION_01(N_POP, D, X_L, X_U)
-        for I in range(N_POP):
-            OF[I, 0] = OF_FUNCTION(X[I, :], NULL_DIC)
-            FIT[I, 0] = META_CO.FIT_VALUE(OF[I, 0])
-            NEOF_COUNT += 1
-      
-        # Initial temperature
-        if TEMP_INI is None:
-            TEMPERATURE = META_SA.START_TEMPERATURE(OF_FUNCTION, NULL_DIC, N_POP, D, X_L, X_U, X, OF, SIGMA)                      
-        else:
-            TEMPERATURE = TEMP_INI
-                       
-        # Storage all values in RESULTS_ITER
-        for I, X_ALL, OF_ALL, FIT_ALL, in zip(RESULTS_ITER, X, OF, FIT):
-            I['X_POSITION'][0, :] = X_ALL
-            I['OF'][0] = OF_ALL
-            I['FIT'][0] = FIT_ALL
-            I['PARAMETERS'][0] = TEMPERATURE
-            I['NEOF'][0] = NEOF_COUNT
-        
-        # Best, average and worst storage
-        BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
-        BEST_ITER['ID_PARTICLE'][0] = BEST_POSITION
-        WORST_ITER['ID_PARTICLE'][0] = WORST_POSITION
-        BEST_ITER['X_POSITION'][0, :] = X_BEST
-        WORST_ITER['X_POSITION'][0, :] = X_WORST
-        BEST_ITER['OF'][0] = OF_BEST
-        AVERAGE_ITER['OF'][0] = OF_AVERAGE
-        WORST_ITER['OF'][0] = OF_WORST
-        BEST_ITER['FIT'][0] = FIT_BEST
-        AVERAGE_ITER['FIT'][0] = FIT_AVERAGE
-        WORST_ITER['FIT'][0] = FIT_WORST
-        BEST_ITER['PARAMETERS'][0] = TEMPERATURE
-        BEST_ITER['NEOF'][0] = NEOF_COUNT
-        AVERAGE_ITER['NEOF'][0] = NEOF_COUNT
-        WORST_ITER['NEOF'][0] = NEOF_COUNT
-        
-        # Iteration procedure
-        for ITER in range(N_ITER):
-
-            # Population movement
-            for POP in range(N_POP):
-                
-                # Simulated Annealing particle movement (Same Hill Climbing movement)
-                X_ITEMP, OF_ITEMP, FIT_ITEMP, NEOF = META_HC.HC_MOVEMENT(OF_FUNCTION, NULL_DIC, X[POP, :], X_L, X_U, D, SIGMA) 
-                
-                # Energy
-                DELTAE = OF_ITEMP - OF[POP, 0]
-                
-                # Probability of acceptance of the movement
-                if DELTAE < 0:
-                    PROBABILITY_STATE = 1
-                elif DELTAE >= 0:
-                    PROBABILITY_STATE = np.exp(- DELTAE / TEMPERATURE)
-                
-                # New design variables
-                RANDON_NUMBER = np.random.random()
-                if RANDON_NUMBER < PROBABILITY_STATE:
-                    X[POP, :] = X_ITEMP
-                    OF[POP, 0] = OF_ITEMP
-                    FIT[POP, 0] = FIT_ITEMP
-                else:
-                    pass
-                
-                # Update NEOF (Number of Objective Function Evaluations)
-                NEOF_COUNT += NEOF
-            
-            # Storage all values in RESULTS_ITER
-            for I, X_ALL, OF_ALL, FIT_ALL  in zip(RESULTS_ITER, X, OF, FIT):
-                I['X_POSITION'][ITER + 1, :] = X_ALL
-                I['OF'][ITER + 1] = OF_ALL
-                I['FIT'][ITER + 1] = FIT_ALL
-                I['PARAMETERS'][ITER + 1] = TEMPERATURE
-                I['NEOF'][ITER + 1] = NEOF_COUNT
-            
-            # Best, average and worst storage
-            BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
-            BEST_ITER['ID_PARTICLE'][ITER + 1] = BEST_POSITION
-            WORST_ITER['ID_PARTICLE'][ITER + 1] = WORST_POSITION
-            BEST_ITER['X_POSITION'][ITER + 1, :] = X_BEST
-            WORST_ITER['X_POSITION'][ITER + 1, :] = X_WORST
-            BEST_ITER['OF'][ITER + 1] = OF_BEST
-            AVERAGE_ITER['OF'][ITER + 1] = OF_AVERAGE
-            WORST_ITER['OF'][ITER + 1] = OF_WORST
-            BEST_ITER['FIT'][ITER + 1] = FIT_BEST
-            AVERAGE_ITER['FIT'][ITER + 1] = FIT_AVERAGE
-            WORST_ITER['FIT'][ITER + 1] = FIT_WORST
-            BEST_ITER['PARAMETERS'][ITER + 1] = TEMPERATURE
-            BEST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
-            AVERAGE_ITER['NEOF'][ITER + 1] = NEOF_COUNT
-            WORST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
-
-            # Update temperature
-            # https://pdfs.semanticscholar.org/da04/e9aa59e9bac1926c2ee776fc8881566739c4.pdf
-            # Geometric cooling scheme
-            if SCHEDULE == 'GEOMETRIC':
-                TEMPERATURE = TEMPERATURE * ALPHA
-            # Lundy cooling scheme
-            elif SCHEDULE == 'LUNDY':
-                TEMPERATURE = TEMPERATURE / (1 + ALPHA * TEMPERATURE) 
-            # Linear cooling scheme
-            elif SCHEDULE == 'LINEAR':
-                TEMPERATURE = TEMPERATURE - ALPHA
-            # Logarithmic cooling scheme
-            elif SCHEDULE == 'LOGARITHMIC':
-                TEMPERATURE = TEMPERATURE / np.log2(ITER + ALPHA)
-        
-        # Append iteration results
-        RESULTS_REP.append(RESULTS_ITER)
-        BEST_REP.append(BEST_ITER)
-        AVERAGE_REP.append(AVERAGE_ITER)
-        WORST_REP.append(WORST_ITER)
-        
-        # Progress bar update
-        time.sleep(0.01)
-        META_CO.PROGRESS_BAR(REP + 1, N_REP)
-    END = time.time()
-    
-    # Resume process (Time and Excel outputs)
-    print('Process Time: %.2f' % (END - INIT), 'Seconds', '\n', 'Seconds per repetition: %.2f' % ((END - INIT) / N_REP))
-    STATUS_PROCEDURE = META_CO.SUMMARY_ANALYSIS(BEST_REP, N_REP, N_ITER)
-    for REP in range(N_REP):
-        NAME.append(MODEL_NAME + 'REP_' + str(REP) + '_BEST_' + str(REP) + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S')))
-        META_CO.EXCEL_WRITER_ITERATION(NAME[REP], D, BEST_REP[REP])
-    NAME_RESUME = MODEL_NAME + 'RESUME' + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S'))
-    META_CO.EXCEL_PROCESS_RESUME(NAME_RESUME, D, BEST_REP, N_ITER, N_REP)    
-    
-    return RESULTS_REP, BEST_REP, AVERAGE_REP, WORST_REP, STATUS_PROCEDURE
-
-def FIREFLY_ALGORITHM_001(OF_FUNCTION, SETUP):
-    """ 
-    Standard Firefly algorithm.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/FA.html
-    """
-    
-    # Setup config
-    N_REP = SETUP['N_REP']
-    N_ITER = SETUP['N_ITER']
-    N_POP = SETUP['N_POP']
-    D = SETUP['D']
-    X_L = SETUP['X_L']
-    X_U = SETUP['X_U']
-    NULL_DIC = SETUP['NULL_DIC']
-    MODEL_NAME = 'META_FA001_'
-    
-    # Parameters
-    PARAMETERS = SETUP['PARAMETERS']
-    BETA_0 = PARAMETERS['BETA_0']
-    ALPHA_MIN = PARAMETERS['ALPHA_MIN']
-    ALPHA_MAX = PARAMETERS['ALPHA_MAX']
-    THETA = PARAMETERS['THETA']
-    GAMMA = PARAMETERS['GAMMA']
-    ALPHA_UPDATE = PARAMETERS['TYPE ALPHA UPDATE']
-    
-    # Creating variables in the repetitions procedure
-    RESULTS_REP = []
-    BEST_REP = []
-    WORST_REP = []
-    AVERAGE_REP = []
-    NAME = []
-    if NULL_DIC == None:
-        NULL_DIC = []
-    else:
-        pass 
-    
-    # Repetition looping
-    INIT = time.time()
-    for REP in range(N_REP):
-        
-        # Creating variables in the iterations procedure
-        OF = np.zeros((N_POP, 1)); 
-        FIT = np.zeros((N_POP, 1))
-        RESULTS_ITER = [{'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': J} for J in range(N_POP)]
-        BEST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
-        AVERAGE_ITER = {'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1)}
-        WORST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
-        NEOF_COUNT = 0 
-        
-        # Initial population
-        X = META_CO.INITIAL_POPULATION_01(N_POP, D, X_L, X_U)
-        for I in range(N_POP):
-            OF[I, 0] = OF_FUNCTION(X[I, :], NULL_DIC)
-            FIT[I, 0] = META_CO.FIT_VALUE(OF[I, 0])
-            NEOF_COUNT += 1
-        
-        # Initial random parameter
-        ALPHA = ALPHA_MAX
-   
-        # Storage all values in RESULTS_ITER
-        for I, X_ALL, OF_ALL, FIT_ALL, in zip(RESULTS_ITER, X, OF, FIT):
-            I['X_POSITION'][0, :] = X_ALL
-            I['OF'][0] = OF_ALL
-            I['FIT'][0] = FIT_ALL
-            I['PARAMETERS'][0] = ALPHA
-            I['NEOF'][0] = NEOF_COUNT
-        
-        # Best, average and worst storage
-        BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
-        BEST_ITER['ID_PARTICLE'][0] = BEST_POSITION
-        WORST_ITER['ID_PARTICLE'][0] = WORST_POSITION
-        BEST_ITER['X_POSITION'][0, :] = X_BEST
-        WORST_ITER['X_POSITION'][0, :] = X_WORST
-        BEST_ITER['OF'][0] = OF_BEST
-        AVERAGE_ITER['OF'][0] = OF_AVERAGE
-        WORST_ITER['OF'][0] = OF_WORST
-        BEST_ITER['FIT'][0] = FIT_BEST
-        AVERAGE_ITER['FIT'][0] = FIT_AVERAGE
-        WORST_ITER['FIT'][0] = FIT_WORST
-        BEST_ITER['PARAMETERS'][0] = ALPHA
-        BEST_ITER['NEOF'][0] = NEOF_COUNT
-        AVERAGE_ITER['NEOF'][0] = NEOF_COUNT
-        WORST_ITER['NEOF'][0] = NEOF_COUNT
-        
-        # Iteration procedure
-        for ITER in range(N_ITER):
-            # Ordering firefly according to fitness
-            X_TEMP = X.copy()
-            OF_TEMP = OF.copy()
-            FIT_TEMP = FIT.copy()
-            SORT_POSITIONS = np.argsort(OF_TEMP.T)
-            
-            for I in range(N_POP):
-                AUX = SORT_POSITIONS[0, I]
-                X[I, :] = X_TEMP[AUX, :]
-                OF[I, 0] = OF_TEMP[AUX, 0] 
-                FIT[I, 0] = FIT_TEMP[AUX, 0]
-            
-            # Population movement
-            X_J = X.copy()
-            FITJ = FIT.copy()
-            for POP_I in range(N_POP):
-                FIT_I = FIT[POP_I, 0]
-                for POP_J in range(N_POP):
-                    FIT_J = FITJ[POP_J, 0]
-                    if FIT_I < FIT_J:
-                        BETA = META_FA.ATTRACTIVENESS_FIREFLY_PARAMETER(BETA_0, GAMMA, X[POP_I, :], X_J[POP_J, :], D)                            
-                        X_ITEMP, OF_ITEMP, FIT_ITEMP, NEOF = META_FA.FIREFLY_MOVEMENT(OF_FUNCTION, X[POP_I, :], X_J[POP_J, :], BETA, ALPHA, D, X_L, X_U, NULL_DIC)
-                    else:
-                        X_ITEMP = X[POP_I, :]
-                        OF_ITEMP = OF[POP_I, 0]
-                        FIT_ITEMP = FIT[POP_I, 0]
-                        NEOF = 0
-                    
-                    # New design variables
-                    X[POP_I, :] = X_ITEMP
-                    OF[POP_I, 0] = OF_ITEMP
-                    FIT[POP_I, 0] = FIT_ITEMP
-                    NEOF_COUNT += NEOF
-            
-            # Storage all values in RESULTS_ITER
-            for I, X_ALL, OF_ALL, FIT_ALL  in zip(RESULTS_ITER, X, OF, FIT):
-                I['X_POSITION'][ITER + 1, :] = X_ALL
-                I['OF'][ITER + 1] = OF_ALL
-                I['FIT'][ITER + 1] = FIT_ALL
-                I['PARAMETERS'][ITER + 1] = ALPHA
-                I['NEOF'][ITER + 1] = NEOF_COUNT
-            
-            # Best, average and worst storage
-            BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
-            BEST_ITER['ID_PARTICLE'][ITER + 1] = BEST_POSITION
-            WORST_ITER['ID_PARTICLE'][ITER + 1] = WORST_POSITION
-            BEST_ITER['X_POSITION'][ITER + 1, :] = X_BEST
-            WORST_ITER['X_POSITION'][ITER + 1, :] = X_WORST
-            BEST_ITER['OF'][ITER + 1] = OF_BEST
-            AVERAGE_ITER['OF'][ITER + 1] = OF_AVERAGE
-            WORST_ITER['OF'][ITER + 1] = OF_WORST
-            BEST_ITER['FIT'][ITER + 1] = FIT_BEST
-            AVERAGE_ITER['FIT'][ITER + 1] = FIT_AVERAGE
-            WORST_ITER['FIT'][ITER + 1] = FIT_WORST
-            BEST_ITER['PARAMETERS'][ITER + 1] = ALPHA
-            BEST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
-            AVERAGE_ITER['NEOF'][ITER + 1] = NEOF_COUNT
-            WORST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
-
-            # Update random parameter
-            if ALPHA_UPDATE == 'YANG 0':
-                ALPHA = ALPHA_MIN + (ALPHA_MAX - ALPHA_MIN) * THETA ** ITER
-            elif ALPHA_UPDATE == 'YANG 1':
-                ALPHA = ALPHA_MAX * THETA ** ITER      
-        
-        # Append iteration results
-        RESULTS_REP.append(RESULTS_ITER)
-        BEST_REP.append(BEST_ITER)
-        AVERAGE_REP.append(AVERAGE_ITER)
-        WORST_REP.append(WORST_ITER)
-        
-        # Progress bar update
-        time.sleep(0.01)
-        META_CO.PROGRESS_BAR(REP + 1, N_REP)
-    END = time.time()
-    
-    # Resume process (Time and Excel outputs)
-    print('Process Time: %.2f' % (END - INIT), 'Seconds', '\n', 'Seconds per repetition: %.2f' % ((END - INIT) / N_REP))
-    STATUS_PROCEDURE = META_CO.SUMMARY_ANALYSIS(BEST_REP, N_REP, N_ITER)
-    for REP in range(N_REP):
-        NAME.append(MODEL_NAME + 'REP_' + str(REP) + '_BEST_' + str(REP) + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S')))
-        META_CO.EXCEL_WRITER_ITERATION(NAME[REP], D, BEST_REP[REP])
-    NAME_RESUME = MODEL_NAME + 'RESUME' + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S'))
-    META_CO.EXCEL_PROCESS_RESUME(NAME_RESUME, D, BEST_REP, N_ITER, N_REP)    
-    
-    return RESULTS_REP, BEST_REP, AVERAGE_REP, WORST_REP, STATUS_PROCEDURE
-
-def PSO_ALGORITHM_001(OF_FUNCTION, SETUP):
-    """ 
-    Standard Hill climbing algorithm. Continuous version. The algorithm also presents the results formatted in a spreadsheet.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/HC.html
-    """
-    
-    # Setup config
-    N_REP = SETUP['N_REP']
-    N_ITER = SETUP['N_ITER']
-    N_POP = SETUP['N_POP']
-    D = SETUP['D']
-    X_L = SETUP['X_L']
-    X_U = SETUP['X_U']
-    NULL_DIC = SETUP['NULL_DIC']
-    MODEL_NAME = 'META_HC001_'
-
-    # Parameters
-    PARAMETERS = SETUP['PARAMETERS']
-    SIGMA = (PARAMETERS['SIGMA'] / 100)
-    
-    # Creating variables in the repetitions procedure
-    RESULTS_REP = []
-    BEST_REP = []
-    WORST_REP = []
-    AVERAGE_REP = []
-    NAME = []
-    if NULL_DIC == None:
-        NULL_DIC = []
-    else:
-        pass 
-    
-    # Repetition looping
-    INIT = time.time()
-    for REP in range(N_REP):
-        
-        # Creating variables in the iterations procedure
-        OF = np.zeros((N_POP, 1)); 
-        FIT = np.zeros((N_POP, 1))
-        RESULTS_ITER = [{'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': J} for J in range(N_POP)]
-        BEST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
-        AVERAGE_ITER = {'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1)}
-        WORST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
-        NEOF_COUNT = 0 
-        
-        # Initial population
-        X = META_CO.INITIAL_POPULATION_01(N_POP, D, X_L, X_U)
-        for I in range(N_POP):
-            OF[I, 0] = OF_FUNCTION(X[I, :], NULL_DIC)
-            FIT[I, 0] = META_CO.FIT_VALUE(OF[I, 0])
-            NEOF_COUNT += 1
-               
-        # Storage all values in RESULTS_ITER
-        for I, X_ALL, OF_ALL, FIT_ALL, in zip(RESULTS_ITER, X, OF, FIT):
-            I['X_POSITION'][0, :] = X_ALL
-            I['OF'][0] = OF_ALL
-            I['FIT'][0] = FIT_ALL
-            I['PARAMETERS'][0] = None
-            I['NEOF'][0] = NEOF_COUNT
-        
-        # Best, average and worst storage
-        BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
-        BEST_ITER['ID_PARTICLE'][0] = BEST_POSITION
-        WORST_ITER['ID_PARTICLE'][0] = WORST_POSITION
-        BEST_ITER['X_POSITION'][0, :] = X_BEST
-        WORST_ITER['X_POSITION'][0, :] = X_WORST
-        BEST_ITER['OF'][0] = OF_BEST
-        AVERAGE_ITER['OF'][0] = OF_AVERAGE
-        WORST_ITER['OF'][0] = OF_WORST
-        BEST_ITER['FIT'][0] = FIT_BEST
-        AVERAGE_ITER['FIT'][0] = FIT_AVERAGE
-        WORST_ITER['FIT'][0] = FIT_WORST
-        BEST_ITER['PARAMETERS'][0] = None
-        BEST_ITER['NEOF'][0] = NEOF_COUNT
-        AVERAGE_ITER['NEOF'][0] = NEOF_COUNT
-        WORST_ITER['NEOF'][0] = NEOF_COUNT
-        
-        # Iteration procedure
-        for ITER in range(N_ITER):
-
-            # Population movement
-            for POP in range(N_POP):
-                
-                # Hill Climbing particle movement
-                X_ITEMP, OF_ITEMP, FIT_ITEMP, NEOF = META_HC.HC_MOVEMENT(OF_FUNCTION, NULL_DIC, X[POP, :], X_L, X_U, D, SIGMA) 
-                
-                # New design variables
-                if FIT_ITEMP > FIT[POP, 0]:
-                    X[POP, :] = X_ITEMP
-                    OF[POP, 0] = OF_ITEMP
-                    FIT[POP, 0] = FIT_ITEMP
-                else:
-                    pass
-                
-                # Update NEOF (Number of Objective Function Evaluations)
-                NEOF_COUNT += NEOF
-            
-            # Storage all values in RESULTS_ITER
-            for I, X_ALL, OF_ALL, FIT_ALL  in zip(RESULTS_ITER, X, OF, FIT):
-                I['X_POSITION'][ITER + 1, :] = X_ALL
-                I['OF'][ITER + 1] = OF_ALL
-                I['FIT'][ITER + 1] = FIT_ALL
-                I['PARAMETERS'][ITER + 1] = None
-                I['NEOF'][ITER + 1] = NEOF_COUNT
-            
-            # Best, average and worst storage
-            BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
-            BEST_ITER['ID_PARTICLE'][ITER + 1] = BEST_POSITION
-            WORST_ITER['ID_PARTICLE'][ITER + 1] = WORST_POSITION
-            BEST_ITER['X_POSITION'][ITER + 1, :] = X_BEST
-            WORST_ITER['X_POSITION'][ITER + 1, :] = X_WORST
-            BEST_ITER['OF'][ITER + 1] = OF_BEST
-            AVERAGE_ITER['OF'][ITER + 1] = OF_AVERAGE
-            WORST_ITER['OF'][ITER + 1] = OF_WORST
-            BEST_ITER['FIT'][ITER + 1] = FIT_BEST
-            AVERAGE_ITER['FIT'][ITER + 1] = FIT_AVERAGE
-            WORST_ITER['FIT'][ITER + 1] = FIT_WORST
-            BEST_ITER['PARAMETERS'][ITER + 1] = None
-            BEST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
-            AVERAGE_ITER['NEOF'][ITER + 1] = NEOF_COUNT
-            WORST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
-        
-        # Append iteration results
-        RESULTS_REP.append(RESULTS_ITER)
-        BEST_REP.append(BEST_ITER)
-        AVERAGE_REP.append(AVERAGE_ITER)
-        WORST_REP.append(WORST_ITER)
-        
-        # Progress bar update
-        time.sleep(0.01)
-        META_CO.PROGRESS_BAR(REP + 1, N_REP)
-    END = time.time()
-    
-    # Resume process (Time and Excel outputs)
-    print('Process Time: %.2f' % (END - INIT), 'Seconds', '\n', 'Seconds per repetition: %.2f' % ((END - INIT) / N_REP))
-    STATUS_PROCEDURE = META_CO.SUMMARY_ANALYSIS(BEST_REP, N_REP, N_ITER)
-    for REP in range(N_REP):
-        NAME.append(MODEL_NAME + 'REP_' + str(REP) + '_BEST_' + str(REP) + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S')))
-        META_CO.EXCEL_WRITER_ITERATION(NAME[REP], D, BEST_REP[REP])
-    NAME_RESUME = MODEL_NAME + 'RESUME' + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S'))
-    META_CO.EXCEL_PROCESS_RESUME(NAME_RESUME, D, BEST_REP, N_ITER, N_REP)    
-    
-    return RESULTS_REP, BEST_REP, AVERAGE_REP, WORST_REP, STATUS_PROCEDURE
+import numpy as np
+import time
+import META_TOOLBOX.META_CO_LIBRARY as META_CO
+import META_TOOLBOX.META_HC_LIBRARY as META_HC
+import META_TOOLBOX.META_SA_LIBRARY as META_SA
+import META_TOOLBOX.META_FA_LIBRARY as META_FA
+import META_TOOLBOX.META_DE_LIBRARY as META_DE
+import META_TOOLBOX.META_GA_LIBRARY as META_GA
+import META_TOOLBOX.META_PSO_LIBRARY as META_PSO
+from datetime import datetime
+
+def HELLO():
+    """
+    Test function.
+    """
+    print("hello world")
+    return
+
+def HILL_CLIMBING_001(OF_FUNCTION, SETUP):
+    """ 
+    Standard Hill climbing algorithm. Continuous version. The algorithm also presents the results formatted in a spreadsheet.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/HC.html
+    """
+    
+    # Setup config
+    N_REP = SETUP['N_REP']
+    N_ITER = SETUP['N_ITER']
+    N_POP = SETUP['N_POP']
+    D = SETUP['D']
+    X_L = SETUP['X_L']
+    X_U = SETUP['X_U']
+    NULL_DIC = SETUP['NULL_DIC']
+    MODEL_NAME = 'META_HC001_'
+
+    # Parameters
+    PARAMETERS = SETUP['PARAMETERS']
+    SIGMA = PARAMETERS['PERCENTAGE STD (SIGMA)'] / 100
+    
+    # Creating variables in the repetitions procedure
+    RESULTS_REP = []
+    BEST_REP = []
+    WORST_REP = []
+    AVERAGE_REP = []
+    NAME = []
+    if NULL_DIC == None:
+        NULL_DIC = []
+    else:
+        pass 
+    
+    # Repetition looping
+    INIT = time.time()
+    for REP in range(N_REP):
+        
+        # Creating variables in the iterations procedure
+        OF = np.zeros((N_POP, 1)); 
+        FIT = np.zeros((N_POP, 1))
+        RESULTS_ITER = [{'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': J} for J in range(N_POP)]
+        BEST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
+        AVERAGE_ITER = {'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1)}
+        WORST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
+        NEOF_COUNT = 0 
+        
+        # Initial population
+        X = META_CO.INITIAL_POPULATION_01(N_POP, D, X_L, X_U)
+        for I in range(N_POP):
+            OF[I, 0] = OF_FUNCTION(X[I, :], NULL_DIC)
+            FIT[I, 0] = META_CO.FIT_VALUE(OF[I, 0])
+            NEOF_COUNT += 1
+               
+        # Storage all values in RESULTS_ITER
+        for I, X_ALL, OF_ALL, FIT_ALL, in zip(RESULTS_ITER, X, OF, FIT):
+            I['X_POSITION'][0, :] = X_ALL
+            I['OF'][0] = OF_ALL
+            I['FIT'][0] = FIT_ALL
+            I['PARAMETERS'][0] = None
+            I['NEOF'][0] = NEOF_COUNT
+        
+        # Best, average and worst storage
+        BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
+        BEST_ITER['ID_PARTICLE'][0] = BEST_POSITION
+        WORST_ITER['ID_PARTICLE'][0] = WORST_POSITION
+        BEST_ITER['X_POSITION'][0, :] = X_BEST
+        WORST_ITER['X_POSITION'][0, :] = X_WORST
+        BEST_ITER['OF'][0] = OF_BEST
+        AVERAGE_ITER['OF'][0] = OF_AVERAGE
+        WORST_ITER['OF'][0] = OF_WORST
+        BEST_ITER['FIT'][0] = FIT_BEST
+        AVERAGE_ITER['FIT'][0] = FIT_AVERAGE
+        WORST_ITER['FIT'][0] = FIT_WORST
+        BEST_ITER['PARAMETERS'][0] = None
+        BEST_ITER['NEOF'][0] = NEOF_COUNT
+        AVERAGE_ITER['NEOF'][0] = NEOF_COUNT
+        WORST_ITER['NEOF'][0] = NEOF_COUNT
+        
+        # Iteration procedure
+        for ITER in range(N_ITER):
+
+            # Population movement
+            for POP in range(N_POP):
+                
+                # Hill Climbing particle movement
+                X_ITEMP, OF_ITEMP, FIT_ITEMP, NEOF = META_HC.HC_MOVEMENT(OF_FUNCTION, NULL_DIC, X[POP, :], X_L, X_U, D, SIGMA) 
+                
+                # New design variables
+                if FIT_ITEMP > FIT[POP, 0]:
+                    X[POP, :] = X_ITEMP
+                    OF[POP, 0] = OF_ITEMP
+                    FIT[POP, 0] = FIT_ITEMP
+                else:
+                    pass
+                
+                # Update NEOF (Number of Objective Function Evaluations)
+                NEOF_COUNT += NEOF
+            
+            # Storage all values in RESULTS_ITER
+            for I, X_ALL, OF_ALL, FIT_ALL  in zip(RESULTS_ITER, X, OF, FIT):
+                I['X_POSITION'][ITER + 1, :] = X_ALL
+                I['OF'][ITER + 1] = OF_ALL
+                I['FIT'][ITER + 1] = FIT_ALL
+                I['PARAMETERS'][ITER + 1] = None
+                I['NEOF'][ITER + 1] = NEOF_COUNT
+            
+            # Best, average and worst storage
+            BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
+            BEST_ITER['ID_PARTICLE'][ITER + 1] = BEST_POSITION
+            WORST_ITER['ID_PARTICLE'][ITER + 1] = WORST_POSITION
+            BEST_ITER['X_POSITION'][ITER + 1, :] = X_BEST
+            WORST_ITER['X_POSITION'][ITER + 1, :] = X_WORST
+            BEST_ITER['OF'][ITER + 1] = OF_BEST
+            AVERAGE_ITER['OF'][ITER + 1] = OF_AVERAGE
+            WORST_ITER['OF'][ITER + 1] = OF_WORST
+            BEST_ITER['FIT'][ITER + 1] = FIT_BEST
+            AVERAGE_ITER['FIT'][ITER + 1] = FIT_AVERAGE
+            WORST_ITER['FIT'][ITER + 1] = FIT_WORST
+            BEST_ITER['PARAMETERS'][ITER + 1] = None
+            BEST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
+            AVERAGE_ITER['NEOF'][ITER + 1] = NEOF_COUNT
+            WORST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
+        
+        # Append iteration results
+        RESULTS_REP.append(RESULTS_ITER)
+        BEST_REP.append(BEST_ITER)
+        AVERAGE_REP.append(AVERAGE_ITER)
+        WORST_REP.append(WORST_ITER)
+        
+        # Progress bar update
+        time.sleep(0.01)
+        META_CO.PROGRESS_BAR(REP + 1, N_REP)
+    END = time.time()
+    
+    # Resume process (Time and Excel outputs)
+    print('Process Time: %.2f' % (END - INIT), 'Seconds', '\n', 'Seconds per repetition: %.2f' % ((END - INIT) / N_REP))
+    STATUS_PROCEDURE = META_CO.SUMMARY_ANALYSIS(BEST_REP, N_REP, N_ITER)
+    for REP in range(N_REP):
+        NAME.append(MODEL_NAME + 'REP_' + str(REP) + '_BEST_' + str(REP) + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S')))
+        META_CO.EXCEL_WRITER_ITERATION(NAME[REP], D, BEST_REP[REP])
+    NAME_RESUME = MODEL_NAME + 'RESUME' + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S'))
+    META_CO.EXCEL_PROCESS_RESUME(NAME_RESUME, D, BEST_REP, N_ITER, N_REP)    
+    
+    return RESULTS_REP, BEST_REP, AVERAGE_REP, WORST_REP, STATUS_PROCEDURE
+
+def SIMULATED_ANNEALING_001(OF_FUNCTION, SETUP):
+    """ 
+    Standard Simulated annealing algorithm. Continuous version. The algorithm also presents the results formatted in a spreadsheet.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/SA001.html
+    """
+    
+    # Setup config
+    N_REP = SETUP['N_REP']
+    N_ITER = SETUP['N_ITER']
+    N_POP = SETUP['N_POP']
+    D = SETUP['D']
+    X_L = SETUP['X_L']
+    X_U = SETUP['X_U']
+    NULL_DIC = SETUP['NULL_DIC']
+    MODEL_NAME = 'META_SA001_'
+
+    # Parameters
+    PARAMETERS = SETUP['PARAMETERS']
+    SIGMA = PARAMETERS['PERCENTAGE STD (SIGMA)'] / 100
+    SCHEDULE = PARAMETERS['COOLING SCHEME']
+    ALPHA = PARAMETERS['TEMP. UPDATE (ALPHA)']
+    TEMP_INI = PARAMETERS['INITIAL TEMP. (T_0)']
+        
+    # Creating variables in the repetitions procedure
+    RESULTS_REP = []
+    BEST_REP = []
+    WORST_REP = []
+    AVERAGE_REP = []
+    NAME = []
+    if NULL_DIC == None:
+        NULL_DIC = []
+    else:
+        pass 
+    
+    # Repetition looping
+    INIT = time.time()
+    for REP in range(N_REP):
+        
+        # Creating variables in the iterations procedure
+        OF = np.zeros((N_POP, 1)); 
+        FIT = np.zeros((N_POP, 1))
+        RESULTS_ITER = [{'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': J} for J in range(N_POP)]
+        BEST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
+        AVERAGE_ITER = {'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1)}
+        WORST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
+        NEOF_COUNT = 0 
+        
+        # Initial population
+        X = META_CO.INITIAL_POPULATION_01(N_POP, D, X_L, X_U)
+        for I in range(N_POP):
+            OF[I, 0] = OF_FUNCTION(X[I, :], NULL_DIC)
+            FIT[I, 0] = META_CO.FIT_VALUE(OF[I, 0])
+            NEOF_COUNT += 1
+      
+        # Initial temperature
+        if TEMP_INI is None:
+            TEMPERATURE = META_SA.START_TEMPERATURE(OF_FUNCTION, NULL_DIC, N_POP, D, X_L, X_U, X, OF, SIGMA)                      
+        else:
+            TEMPERATURE = TEMP_INI
+                       
+        # Storage all values in RESULTS_ITER
+        for I, X_ALL, OF_ALL, FIT_ALL, in zip(RESULTS_ITER, X, OF, FIT):
+            I['X_POSITION'][0, :] = X_ALL
+            I['OF'][0] = OF_ALL
+            I['FIT'][0] = FIT_ALL
+            I['PARAMETERS'][0] = TEMPERATURE
+            I['NEOF'][0] = NEOF_COUNT
+        
+        # Best, average and worst storage
+        BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
+        BEST_ITER['ID_PARTICLE'][0] = BEST_POSITION
+        WORST_ITER['ID_PARTICLE'][0] = WORST_POSITION
+        BEST_ITER['X_POSITION'][0, :] = X_BEST
+        WORST_ITER['X_POSITION'][0, :] = X_WORST
+        BEST_ITER['OF'][0] = OF_BEST
+        AVERAGE_ITER['OF'][0] = OF_AVERAGE
+        WORST_ITER['OF'][0] = OF_WORST
+        BEST_ITER['FIT'][0] = FIT_BEST
+        AVERAGE_ITER['FIT'][0] = FIT_AVERAGE
+        WORST_ITER['FIT'][0] = FIT_WORST
+        BEST_ITER['PARAMETERS'][0] = TEMPERATURE
+        BEST_ITER['NEOF'][0] = NEOF_COUNT
+        AVERAGE_ITER['NEOF'][0] = NEOF_COUNT
+        WORST_ITER['NEOF'][0] = NEOF_COUNT
+        
+        # Iteration procedure
+        for ITER in range(N_ITER):
+
+            # Population movement
+            for POP in range(N_POP):
+                
+                # Simulated Annealing particle movement (Same Hill Climbing movement)
+                X_ITEMP, OF_ITEMP, FIT_ITEMP, NEOF = META_HC.HC_MOVEMENT(OF_FUNCTION, NULL_DIC, X[POP, :], X_L, X_U, D, SIGMA) 
+                
+                # Energy
+                DELTAE = OF_ITEMP - OF[POP, 0]
+                
+                # Probability of acceptance of the movement
+                if DELTAE < 0:
+                    PROBABILITY_STATE = 1
+                elif DELTAE >= 0:
+                    PROBABILITY_STATE = np.exp(- DELTAE / TEMPERATURE)
+                
+                # New design variables
+                RANDON_NUMBER = np.random.random()
+                if RANDON_NUMBER < PROBABILITY_STATE:
+                    X[POP, :] = X_ITEMP
+                    OF[POP, 0] = OF_ITEMP
+                    FIT[POP, 0] = FIT_ITEMP
+                else:
+                    pass
+                
+                # Update NEOF (Number of Objective Function Evaluations)
+                NEOF_COUNT += NEOF
+            
+            # Storage all values in RESULTS_ITER
+            for I, X_ALL, OF_ALL, FIT_ALL  in zip(RESULTS_ITER, X, OF, FIT):
+                I['X_POSITION'][ITER + 1, :] = X_ALL
+                I['OF'][ITER + 1] = OF_ALL
+                I['FIT'][ITER + 1] = FIT_ALL
+                I['PARAMETERS'][ITER + 1] = TEMPERATURE
+                I['NEOF'][ITER + 1] = NEOF_COUNT
+            
+            # Best, average and worst storage
+            BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
+            BEST_ITER['ID_PARTICLE'][ITER + 1] = BEST_POSITION
+            WORST_ITER['ID_PARTICLE'][ITER + 1] = WORST_POSITION
+            BEST_ITER['X_POSITION'][ITER + 1, :] = X_BEST
+            WORST_ITER['X_POSITION'][ITER + 1, :] = X_WORST
+            BEST_ITER['OF'][ITER + 1] = OF_BEST
+            AVERAGE_ITER['OF'][ITER + 1] = OF_AVERAGE
+            WORST_ITER['OF'][ITER + 1] = OF_WORST
+            BEST_ITER['FIT'][ITER + 1] = FIT_BEST
+            AVERAGE_ITER['FIT'][ITER + 1] = FIT_AVERAGE
+            WORST_ITER['FIT'][ITER + 1] = FIT_WORST
+            BEST_ITER['PARAMETERS'][ITER + 1] = TEMPERATURE
+            BEST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
+            AVERAGE_ITER['NEOF'][ITER + 1] = NEOF_COUNT
+            WORST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
+
+            # Update temperature
+            # https://pdfs.semanticscholar.org/da04/e9aa59e9bac1926c2ee776fc8881566739c4.pdf
+            # Geometric cooling scheme
+            if SCHEDULE == 'GEOMETRIC':
+                TEMPERATURE = TEMPERATURE * ALPHA
+            # Lundy cooling scheme
+            elif SCHEDULE == 'LUNDY':
+                TEMPERATURE = TEMPERATURE / (1 + ALPHA * TEMPERATURE) 
+            # Linear cooling scheme
+            elif SCHEDULE == 'LINEAR':
+                TEMPERATURE = TEMPERATURE - ALPHA
+            # Logarithmic cooling scheme
+            elif SCHEDULE == 'LOGARITHMIC':
+                TEMPERATURE = TEMPERATURE / np.log2(ITER + ALPHA)
+        
+        # Append iteration results
+        RESULTS_REP.append(RESULTS_ITER)
+        BEST_REP.append(BEST_ITER)
+        AVERAGE_REP.append(AVERAGE_ITER)
+        WORST_REP.append(WORST_ITER)
+        
+        # Progress bar update
+        time.sleep(0.01)
+        META_CO.PROGRESS_BAR(REP + 1, N_REP)
+    END = time.time()
+    
+    # Resume process (Time and Excel outputs)
+    print('Process Time: %.2f' % (END - INIT), 'Seconds', '\n', 'Seconds per repetition: %.2f' % ((END - INIT) / N_REP))
+    STATUS_PROCEDURE = META_CO.SUMMARY_ANALYSIS(BEST_REP, N_REP, N_ITER)
+    for REP in range(N_REP):
+        NAME.append(MODEL_NAME + 'REP_' + str(REP) + '_BEST_' + str(REP) + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S')))
+        META_CO.EXCEL_WRITER_ITERATION(NAME[REP], D, BEST_REP[REP])
+    NAME_RESUME = MODEL_NAME + 'RESUME' + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S'))
+    META_CO.EXCEL_PROCESS_RESUME(NAME_RESUME, D, BEST_REP, N_ITER, N_REP)    
+    
+    return RESULTS_REP, BEST_REP, AVERAGE_REP, WORST_REP, STATUS_PROCEDURE
+
+def FIREFLY_ALGORITHM_001(OF_FUNCTION, SETUP):
+    """ 
+    Standard Firefly algorithm.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/FA.html
+    """
+    
+    # Setup config
+    N_REP = SETUP['N_REP']
+    N_ITER = SETUP['N_ITER']
+    N_POP = SETUP['N_POP']
+    D = SETUP['D']
+    X_L = SETUP['X_L']
+    X_U = SETUP['X_U']
+    NULL_DIC = SETUP['NULL_DIC']
+    MODEL_NAME = 'META_FA001_'
+    
+    # Parameters
+    PARAMETERS = SETUP['PARAMETERS']
+    BETA_0 = PARAMETERS['ATTRACTIVENESS (BETA_0)']
+    ALPHA_MIN = PARAMETERS['MIN. RANDOM FACTOR (ALPHA_MIN)']
+    ALPHA_MAX = PARAMETERS['MAX. RANDOM FACTOR (ALPHA_MAX)']
+    THETA = PARAMETERS['THETA']
+    GAMMA = PARAMETERS['LIGHT ABSORPTION (GAMMA)']
+    ALPHA_UPDATE = PARAMETERS['TYPE ALPHA UPDATE']
+    SCALING = PARAMETERS['SCALING (S_D)']
+    
+    # Creating variables in the repetitions procedure
+    RESULTS_REP = []
+    BEST_REP = []
+    WORST_REP = []
+    AVERAGE_REP = []
+    NAME = []
+    if NULL_DIC == None:
+        NULL_DIC = []
+    else:
+        pass 
+    
+    # Repetition looping
+    INIT = time.time()
+    for REP in range(N_REP):
+        
+        # Creating variables in the iterations procedure
+        OF = np.zeros((N_POP, 1)); 
+        FIT = np.zeros((N_POP, 1))
+        RESULTS_ITER = [{'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': J} for J in range(N_POP)]
+        BEST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
+        AVERAGE_ITER = {'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1)}
+        WORST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
+        NEOF_COUNT = 0 
+        
+        # Initial population
+        X = META_CO.INITIAL_POPULATION_01(N_POP, D, X_L, X_U)
+        for I in range(N_POP):
+            OF[I, 0] = OF_FUNCTION(X[I, :], NULL_DIC)
+            FIT[I, 0] = META_CO.FIT_VALUE(OF[I, 0])
+            NEOF_COUNT += 1
+        
+        # Initial random parameter
+        ALPHA = ALPHA_MAX
+   
+        # Storage all values in RESULTS_ITER
+        for I, X_ALL, OF_ALL, FIT_ALL, in zip(RESULTS_ITER, X, OF, FIT):
+            I['X_POSITION'][0, :] = X_ALL
+            I['OF'][0] = OF_ALL
+            I['FIT'][0] = FIT_ALL
+            I['PARAMETERS'][0] = ALPHA
+            I['NEOF'][0] = NEOF_COUNT
+        
+        # Best, average and worst storage
+        BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
+        BEST_ITER['ID_PARTICLE'][0] = BEST_POSITION
+        WORST_ITER['ID_PARTICLE'][0] = WORST_POSITION
+        BEST_ITER['X_POSITION'][0, :] = X_BEST
+        WORST_ITER['X_POSITION'][0, :] = X_WORST
+        BEST_ITER['OF'][0] = OF_BEST
+        AVERAGE_ITER['OF'][0] = OF_AVERAGE
+        WORST_ITER['OF'][0] = OF_WORST
+        BEST_ITER['FIT'][0] = FIT_BEST
+        AVERAGE_ITER['FIT'][0] = FIT_AVERAGE
+        WORST_ITER['FIT'][0] = FIT_WORST
+        BEST_ITER['PARAMETERS'][0] = ALPHA
+        BEST_ITER['NEOF'][0] = NEOF_COUNT
+        AVERAGE_ITER['NEOF'][0] = NEOF_COUNT
+        WORST_ITER['NEOF'][0] = NEOF_COUNT
+        
+        # Iteration procedure
+        for ITER in range(N_ITER):
+            # Ordering firefly according to fitness
+            X_TEMP = X.copy()
+            OF_TEMP = OF.copy()
+            FIT_TEMP = FIT.copy()
+            SORT_POSITIONS = np.argsort(OF_TEMP.T)
+            
+            for I in range(N_POP):
+                AUX = SORT_POSITIONS[0, I]
+                X[I, :] = X_TEMP[AUX, :]
+                OF[I, 0] = OF_TEMP[AUX, 0] 
+                FIT[I, 0] = FIT_TEMP[AUX, 0]
+            
+            # Population movement
+            X_J = X.copy()
+            FITJ = FIT.copy()
+            for POP_I in range(N_POP):
+                FIT_I = FIT[POP_I, 0]
+                for POP_J in range(N_POP):
+                    FIT_J = FITJ[POP_J, 0]
+                    if FIT_I < FIT_J:
+                        BETA = META_FA.ATTRACTIVENESS_FIREFLY_PARAMETER(BETA_0, GAMMA, X[POP_I, :], X_J[POP_J, :], D)                            
+                        X_ITEMP, OF_ITEMP, FIT_ITEMP, NEOF = META_FA.FIREFLY_MOVEMENT(OF_FUNCTION, X[POP_I, :], X_J[POP_J, :], BETA, ALPHA, SCALING, D, X_L, X_U, NULL_DIC)
+                    else:
+                        X_ITEMP = X[POP_I, :]
+                        OF_ITEMP = OF[POP_I, 0]
+                        FIT_ITEMP = FIT[POP_I, 0]
+                        NEOF = 0
+                    
+                    # New design variables
+                    X[POP_I, :] = X_ITEMP
+                    OF[POP_I, 0] = OF_ITEMP
+                    FIT[POP_I, 0] = FIT_ITEMP
+                    NEOF_COUNT += NEOF
+            
+            # Storage all values in RESULTS_ITER
+            for I, X_ALL, OF_ALL, FIT_ALL  in zip(RESULTS_ITER, X, OF, FIT):
+                I['X_POSITION'][ITER + 1, :] = X_ALL
+                I['OF'][ITER + 1] = OF_ALL
+                I['FIT'][ITER + 1] = FIT_ALL
+                I['PARAMETERS'][ITER + 1] = ALPHA
+                I['NEOF'][ITER + 1] = NEOF_COUNT
+            
+            # Best, average and worst storage
+            BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
+            BEST_ITER['ID_PARTICLE'][ITER + 1] = BEST_POSITION
+            WORST_ITER['ID_PARTICLE'][ITER + 1] = WORST_POSITION
+            BEST_ITER['X_POSITION'][ITER + 1, :] = X_BEST
+            WORST_ITER['X_POSITION'][ITER + 1, :] = X_WORST
+            BEST_ITER['OF'][ITER + 1] = OF_BEST
+            AVERAGE_ITER['OF'][ITER + 1] = OF_AVERAGE
+            WORST_ITER['OF'][ITER + 1] = OF_WORST
+            BEST_ITER['FIT'][ITER + 1] = FIT_BEST
+            AVERAGE_ITER['FIT'][ITER + 1] = FIT_AVERAGE
+            WORST_ITER['FIT'][ITER + 1] = FIT_WORST
+            BEST_ITER['PARAMETERS'][ITER + 1] = ALPHA
+            BEST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
+            AVERAGE_ITER['NEOF'][ITER + 1] = NEOF_COUNT
+            WORST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
+
+            # Update random parameter
+            if ALPHA_UPDATE == 'YANG 0':
+                ALPHA = ALPHA_MIN + (ALPHA_MAX - ALPHA_MIN) * THETA ** ITER
+            elif ALPHA_UPDATE == 'YANG 1':
+                ALPHA = ALPHA_MAX * THETA ** ITER      
+            elif ALPHA_UPDATE == 'YANG 2':
+                ALPHA = ALPHA_MAX + (ALPHA_MIN - ALPHA_MAX) * np.exp(- ITER)      
+            elif ALPHA_UPDATE == 'YANG 3':
+                AUX = 1 + np.exp((ITER - N_ITER) / 200)
+                ALPHA = 0.40 / AUX
+            elif ALPHA_UPDATE == 'YANG 4':
+                ALPHA *= 0.99         
+            elif ALPHA_UPDATE == 'YANG 5':
+                ALPHA *= (1 - ITER / N_ITER)  
+            elif ALPHA_UPDATE == 'YANG 6':
+                ALPHA *= (ITER / 9000) ** (1 / ITER)                   
+        # Append iteration results
+        RESULTS_REP.append(RESULTS_ITER)
+        BEST_REP.append(BEST_ITER)
+        AVERAGE_REP.append(AVERAGE_ITER)
+        WORST_REP.append(WORST_ITER)
+        
+        # Progress bar update
+        time.sleep(0.01)
+        META_CO.PROGRESS_BAR(REP + 1, N_REP)
+    END = time.time()
+    
+    # Resume process (Time and Excel outputs)
+    print('Process Time: %.2f' % (END - INIT), 'Seconds', '\n', 'Seconds per repetition: %.2f' % ((END - INIT) / N_REP))
+    STATUS_PROCEDURE = META_CO.SUMMARY_ANALYSIS(BEST_REP, N_REP, N_ITER)
+    for REP in range(N_REP):
+        NAME.append(MODEL_NAME + 'REP_' + str(REP) + '_BEST_' + str(REP) + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S')))
+        META_CO.EXCEL_WRITER_ITERATION(NAME[REP], D, BEST_REP[REP])
+    NAME_RESUME = MODEL_NAME + 'RESUME' + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S'))
+    META_CO.EXCEL_PROCESS_RESUME(NAME_RESUME, D, BEST_REP, N_ITER, N_REP)    
+    
+    return RESULTS_REP, BEST_REP, AVERAGE_REP, WORST_REP, STATUS_PROCEDURE
+
+def PSO_ALGORITHM_001(OF_FUNCTION, SETUP):
+    """ 
+    Standard Particle Swarm Optimization algorithm. Continuous version. The algorithm also presents the results formatted in a spreadsheet.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/PSO.html
+    """
+    
+    # Setup config
+    N_REP = SETUP['N_REP']
+    N_ITER = SETUP['N_ITER']
+    N_POP = SETUP['N_POP']
+    D = SETUP['D']
+    X_L = SETUP['X_L']
+    X_U = SETUP['X_U']
+    NULL_DIC = SETUP['NULL_DIC']
+    MODEL_NAME = 'META_PSO001_'
+
+    # Parameters
+    PARAMETERS = SETUP['PARAMETERS']
+    V_MIN = PARAMETERS['MIN VELOCITY (V_MIN)']
+    V_MAX = PARAMETERS['MAX VELOCITY (V_MAX)']
+    C_1 = PARAMETERS['COGNITIVE COEFFICIENT (C_1)']
+    C_2 = PARAMETERS['SOCIAL COEFFICIENT (C_2)']
+    W_MIN = PARAMETERS['MIN INTERIA (W_MIN)']
+    W_MAX = PARAMETERS['MAX INERTIA (W_MAX)']
+    INERTIA_UPDATE = PARAMETERS['INERTIA UPDATE']
+    
+    # Creating variables in the repetitions procedure
+    RESULTS_REP = []
+    BEST_REP = []
+    WORST_REP = []
+    AVERAGE_REP = []
+    NAME = []
+    if NULL_DIC == None:
+        NULL_DIC = []
+    else:
+        pass 
+    
+    # Repetition looping
+    INIT = time.time()
+    for REP in range(N_REP):
+        
+        # Creating variables in the iterations procedure
+        OF = np.zeros((N_POP, 1)); 
+        FIT = np.zeros((N_POP, 1))
+        RESULTS_ITER = [{'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': J} for J in range(N_POP)]
+        BEST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
+        AVERAGE_ITER = {'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1)}
+        WORST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
+        NEOF_COUNT = 0 
+        
+        # Initial population
+        X = META_CO.INITIAL_POPULATION_01(N_POP, D, X_L, X_U)
+        for I in range(N_POP):
+            OF[I, 0] = OF_FUNCTION(X[I, :], NULL_DIC)
+            FIT[I, 0] = META_CO.FIT_VALUE(OF[I, 0])
+            NEOF_COUNT += 1
+
+        # Initial velociity
+        VEL = META_CO.INITIAL_POPULATION_01(N_POP, D, V_MIN, V_MAX)
+        
+        # Initial random parameter
+        INERTIA = W_MAX
+             
+        # Storage all values in RESULTS_ITER
+        for I, X_ALL, OF_ALL, FIT_ALL, in zip(RESULTS_ITER, X, OF, FIT):
+            I['X_POSITION'][0, :] = X_ALL
+            I['OF'][0] = OF_ALL
+            I['FIT'][0] = FIT_ALL
+            I['PARAMETERS'][0] = INERTIA
+            I['NEOF'][0] = NEOF_COUNT
+        
+        # Best, average and worst storage
+        BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
+        BEST_ITER['ID_PARTICLE'][0] = BEST_POSITION
+        WORST_ITER['ID_PARTICLE'][0] = WORST_POSITION
+        BEST_ITER['X_POSITION'][0, :] = X_BEST
+        WORST_ITER['X_POSITION'][0, :] = X_WORST
+        BEST_ITER['OF'][0] = OF_BEST
+        AVERAGE_ITER['OF'][0] = OF_AVERAGE
+        WORST_ITER['OF'][0] = OF_WORST
+        BEST_ITER['FIT'][0] = FIT_BEST
+        AVERAGE_ITER['FIT'][0] = FIT_AVERAGE
+        WORST_ITER['FIT'][0] = FIT_WORST
+        BEST_ITER['PARAMETERS'][0] = INERTIA
+        BEST_ITER['NEOF'][0] = NEOF_COUNT
+        AVERAGE_ITER['NEOF'][0] = NEOF_COUNT
+        WORST_ITER['NEOF'][0] = NEOF_COUNT
+
+        # Initial PBEST and GBEST
+        P_BEST = X.copy()
+        OF_PBEST = OF.copy()
+        G_BEST = X_BEST.copy()
+        
+        # Iteration procedure
+        for ITER in range(N_ITER):
+
+            # Population movement
+            for POP in range(N_POP):
+                
+                # Particle Swarm Optimization particle movement
+                V_ITEMP, X_ITEMP, OF_ITEMP, FIT_ITEMP, NEOF = META_PSO.PSO_MOVEMENT(OF_FUNCTION, VEL[POP, :], X[POP, :], C_1, C_2, P_BEST[POP, :], G_BEST, D, X_L, X_U, V_MIN, V_MAX, INERTIA, NULL_DIC) 
+
+                # Update PBEST and GBEST
+                P_BEST[POP, :], OF_PBEST[POP, 0] = META_PSO.UPDATE_BEST(X_ITEMP, P_BEST[POP, :], OF_ITEMP, OF_PBEST[POP, 0])
+                               
+                # New design variables
+                VEL[POP, :] = V_ITEMP
+                X[POP, :] = X_ITEMP
+                OF[POP, 0] = OF_ITEMP
+                FIT[POP, 0] = FIT_ITEMP
+               
+                # Update NEOF (Number of Objective Function Evaluations)
+                NEOF_COUNT += NEOF
+            
+            # Storage all values in RESULTS_ITER
+            for I, X_ALL, OF_ALL, FIT_ALL  in zip(RESULTS_ITER, X, OF, FIT):
+                I['X_POSITION'][ITER + 1, :] = X_ALL
+                I['OF'][ITER + 1] = OF_ALL
+                I['FIT'][ITER + 1] = FIT_ALL
+                I['PARAMETERS'][ITER + 1] = None
+                I['NEOF'][ITER + 1] = NEOF_COUNT
+            
+            # GBEST
+            X_BEST = P_BEST[OF_PBEST.argmin(), :]
+            OF_BEST = OF_PBEST[OF_PBEST.argmin(), :]
+            BEST_POSITION = OF_PBEST.argmin()
+
+            # Best, average and worst storage
+            _, WORST_POSITION, _, X_WORST, _, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
+            BEST_ITER['ID_PARTICLE'][ITER + 1] = BEST_POSITION
+            WORST_ITER['ID_PARTICLE'][ITER + 1] = WORST_POSITION
+            BEST_ITER['X_POSITION'][ITER + 1, :] = X_BEST
+            WORST_ITER['X_POSITION'][ITER + 1, :] = X_WORST
+            BEST_ITER['OF'][ITER + 1] = OF_BEST
+            AVERAGE_ITER['OF'][ITER + 1] = OF_AVERAGE
+            WORST_ITER['OF'][ITER + 1] = OF_WORST
+            BEST_ITER['FIT'][ITER + 1] = FIT_BEST
+            AVERAGE_ITER['FIT'][ITER + 1] = FIT_AVERAGE
+            WORST_ITER['FIT'][ITER + 1] = FIT_WORST
+            BEST_ITER['PARAMETERS'][ITER + 1] = None
+            BEST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
+            AVERAGE_ITER['NEOF'][ITER + 1] = NEOF_COUNT
+            WORST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
+        
+            # Update inertia parameter
+            if INERTIA_UPDATE == 'PSO 0':
+                INERTIA = W_MAX
+            elif INERTIA_UPDATE == 'PSO 1':
+                INERTIA = W_MAX - (W_MAX - W_MIN) * (ITER / N_ITER)   
+            elif INERTIA_UPDATE == 'PSO 2':
+                ALPHA = 1 / np.pi() ** 2
+                INERTIA = W_MAX - (W_MAX - W_MIN) * (ITER / N_ITER)  ** ALPHA        
+            elif INERTIA_UPDATE == 'PSO 3':
+                ALPHA = 1 / np.pi() ** 2
+                INERTIA = (2 / N_ITER)  ** 0.30  
+            elif INERTIA_UPDATE == 'PSO 4':
+                INERTIA = W_MIN + (W_MAX - W_MIN) * np.exp((-10 * ITER) / N_ITER)   
+            elif INERTIA_UPDATE == 'PSO 5':
+                INERTIA = W_MAX + (W_MIN - W_MAX) * np.log10(1 + (10 * ITER) / N_ITER)  
+            elif INERTIA_UPDATE == 'PSO 6':
+                INERTIA = 0.50 + np.random.random() / 2 
+
+        # Append iteration results
+        RESULTS_REP.append(RESULTS_ITER)
+        BEST_REP.append(BEST_ITER)
+        AVERAGE_REP.append(AVERAGE_ITER)
+        WORST_REP.append(WORST_ITER)
+        
+        # Progress bar update
+        time.sleep(0.01)
+        META_CO.PROGRESS_BAR(REP + 1, N_REP)
+    END = time.time()
+    
+    # Resume process (Time and Excel outputs)
+    print('Process Time: %.2f' % (END - INIT), 'Seconds', '\n', 'Seconds per repetition: %.2f' % ((END - INIT) / N_REP))
+    STATUS_PROCEDURE = META_CO.SUMMARY_ANALYSIS(BEST_REP, N_REP, N_ITER)
+    for REP in range(N_REP):
+        NAME.append(MODEL_NAME + 'REP_' + str(REP) + '_BEST_' + str(REP) + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S')))
+        META_CO.EXCEL_WRITER_ITERATION(NAME[REP], D, BEST_REP[REP])
+    NAME_RESUME = MODEL_NAME + 'RESUME' + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S'))
+    META_CO.EXCEL_PROCESS_RESUME(NAME_RESUME, D, BEST_REP, N_ITER, N_REP)    
+    
+    return RESULTS_REP, BEST_REP, AVERAGE_REP, WORST_REP, STATUS_PROCEDURE
+
+def DE_ALGORITHM_001(OF_FUNCTION, SETUP):
+    """ 
+    Standard Differential Evolution Optimization algorithm. Continuous version. The algorithm also presents the results formatted in a spreadsheet.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/DE.html
+    """
+    
+    # Setup config
+    N_REP = SETUP['N_REP']
+    N_ITER = SETUP['N_ITER']
+    N_POP = SETUP['N_POP']
+    D = SETUP['D']
+    X_L = SETUP['X_L']
+    X_U = SETUP['X_U']
+    NULL_DIC = SETUP['NULL_DIC']
+    MODEL_NAME = 'META_DE001_'
+
+    # Parameters
+    PARAMETERS = SETUP['PARAMETERS']
+    F = PARAMETERS['MUTATION FACTOR (F)']
+    CR =  PARAMETERS['CROSSOVER RATE (CR)']
+    
+    # Creating variables in the repetitions procedure
+    RESULTS_REP = []
+    BEST_REP = []
+    WORST_REP = []
+    AVERAGE_REP = []
+    NAME = []
+    if NULL_DIC == None:
+        NULL_DIC = []
+    else:
+        pass 
+    
+    # Repetition looping
+    INIT = time.time()
+    for REP in range(N_REP):
+        
+        # Creating variables in the iterations procedure
+        OF = np.zeros((N_POP, 1)); 
+        FIT = np.zeros((N_POP, 1))
+        RESULTS_ITER = [{'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': J} for J in range(N_POP)]
+        BEST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'PARAMETERS': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
+        AVERAGE_ITER = {'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1)}
+        WORST_ITER = {'X_POSITION': np.empty((N_ITER + 1, D)), 'OF': np.empty(N_ITER + 1), 'FIT': np.empty(N_ITER + 1), 'NEOF': np.empty(N_ITER + 1), 'ID_PARTICLE': np.empty(N_ITER + 1)}
+        NEOF_COUNT = 0 
+        
+        # Initial population
+        X = META_CO.INITIAL_POPULATION_01(N_POP, D, X_L, X_U)
+        for I in range(N_POP):
+            OF[I, 0] = OF_FUNCTION(X[I, :], NULL_DIC)
+            FIT[I, 0] = META_CO.FIT_VALUE(OF[I, 0])
+            NEOF_COUNT += 1
+            
+        # Storage all values in RESULTS_ITER
+        for I, X_ALL, OF_ALL, FIT_ALL, in zip(RESULTS_ITER, X, OF, FIT):
+            I['X_POSITION'][0, :] = X_ALL
+            I['OF'][0] = OF_ALL
+            I['FIT'][0] = FIT_ALL
+            I['PARAMETERS'][0] = None
+            I['NEOF'][0] = NEOF_COUNT
+        
+        # Best, average and worst storage
+        BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
+        BEST_ITER['ID_PARTICLE'][0] = BEST_POSITION
+        WORST_ITER['ID_PARTICLE'][0] = WORST_POSITION
+        BEST_ITER['X_POSITION'][0, :] = X_BEST
+        WORST_ITER['X_POSITION'][0, :] = X_WORST
+        BEST_ITER['OF'][0] = OF_BEST
+        AVERAGE_ITER['OF'][0] = OF_AVERAGE
+        WORST_ITER['OF'][0] = OF_WORST
+        BEST_ITER['FIT'][0] = FIT_BEST
+        AVERAGE_ITER['FIT'][0] = FIT_AVERAGE
+        WORST_ITER['FIT'][0] = FIT_WORST
+        BEST_ITER['PARAMETERS'][0] = None
+        BEST_ITER['NEOF'][0] = NEOF_COUNT
+        AVERAGE_ITER['NEOF'][0] = NEOF_COUNT
+        WORST_ITER['NEOF'][0] = NEOF_COUNT
+
+        # Initial PBEST and GBEST
+        P_BEST = X.copy()
+        OF_PBEST = OF.copy()
+        G_BEST = X_BEST.copy()
+        
+        # Iteration procedure
+        for ITER in range(N_ITER):
+
+            # Population movement
+            for POP in range(N_POP):
+                
+                # ID selection
+                IDS_RANDOM = META_DE.SELECTION_ID(N_POP)
+                X_GAMA = X[IDS_RANDOM[0], :]
+                X_BETA = X[IDS_RANDOM[1], :]
+                X_ALFA = X[IDS_RANDOM[2], :]
+
+                # Mutation phase
+                V_TI, _, _, _ = META_GA.MUTATION_OPERATOR_DE_RAND_1(OF_FUNCTION, NULL_DIC, F, X_GAMA, X_BETA, X_ALFA, D, X_L, X_U)
+
+                # Crossover phase
+                X_ITEMP, OF_ITEMP, FIT_ITEMP, NEOF = META_GA.BINOMIAL_CROSSOVER_OPERATOR(OF_FUNCTION, NULL_DIC, V_TI, X[POP, :], CR, D, X_L, X_U)
+
+                # https://www.dca.fee.unicamp.br/~lboccato/topico_11_evolucao_diferencial.pdf
+                # https://edisciplinas.usp.br/pluginfile.php/381792/course/section/113390/aula04.pdf
+                # https://medium.com/eni-digitalks/metaheuristic-optimization-with-the-differential-evolution-algorithm-5301480eca58
+                # https://sci-hub.ru/https://doi.org/10.1016/j.neucom.2020.09.007
+                             
+                # New design variables
+                if FIT_ITEMP > FIT[POP, 0]:
+                    X[POP, :] = X_ITEMP
+                    OF[POP, 0] = OF_ITEMP
+                    FIT[POP, 0] = FIT_ITEMP
+                else:
+                    pass
+               
+                # Update NEOF (Number of Objective Function Evaluations)
+                NEOF_COUNT += NEOF
+            
+            # Storage all values in RESULTS_ITER
+            for I, X_ALL, OF_ALL, FIT_ALL  in zip(RESULTS_ITER, X, OF, FIT):
+                I['X_POSITION'][ITER + 1, :] = X_ALL
+                I['OF'][ITER + 1] = OF_ALL
+                I['FIT'][ITER + 1] = FIT_ALL
+                I['PARAMETERS'][ITER + 1] = None
+                I['NEOF'][ITER + 1] = NEOF_COUNT
+            
+            # Best, average and worst storage
+            BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE = META_CO.BEST_VALUES(X, OF, FIT, N_POP)
+            BEST_ITER['ID_PARTICLE'][ITER + 1] = BEST_POSITION
+            WORST_ITER['ID_PARTICLE'][ITER + 1] = WORST_POSITION
+            BEST_ITER['X_POSITION'][ITER + 1, :] = X_BEST
+            WORST_ITER['X_POSITION'][ITER + 1, :] = X_WORST
+            BEST_ITER['OF'][ITER + 1] = OF_BEST
+            AVERAGE_ITER['OF'][ITER + 1] = OF_AVERAGE
+            WORST_ITER['OF'][ITER + 1] = OF_WORST
+            BEST_ITER['FIT'][ITER + 1] = FIT_BEST
+            AVERAGE_ITER['FIT'][ITER + 1] = FIT_AVERAGE
+            WORST_ITER['FIT'][ITER + 1] = FIT_WORST
+            BEST_ITER['PARAMETERS'][ITER + 1] = None
+            BEST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
+            AVERAGE_ITER['NEOF'][ITER + 1] = NEOF_COUNT
+            WORST_ITER['NEOF'][ITER + 1] = NEOF_COUNT
+              
+        # Append iteration results
+        RESULTS_REP.append(RESULTS_ITER)
+        BEST_REP.append(BEST_ITER)
+        AVERAGE_REP.append(AVERAGE_ITER)
+        WORST_REP.append(WORST_ITER)
+        
+        # Progress bar update
+        time.sleep(0.01)
+        META_CO.PROGRESS_BAR(REP + 1, N_REP)
+    END = time.time()
+    
+    # Resume process (Time and Excel outputs)
+    print('Process Time: %.2f' % (END - INIT), 'Seconds', '\n', 'Seconds per repetition: %.2f' % ((END - INIT) / N_REP))
+    STATUS_PROCEDURE = META_CO.SUMMARY_ANALYSIS(BEST_REP, N_REP, N_ITER)
+    for REP in range(N_REP):
+        NAME.append(MODEL_NAME + 'REP_' + str(REP) + '_BEST_' + str(REP) + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S')))
+        META_CO.EXCEL_WRITER_ITERATION(NAME[REP], D, BEST_REP[REP])
+    NAME_RESUME = MODEL_NAME + 'RESUME' + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S'))
+    META_CO.EXCEL_PROCESS_RESUME(NAME_RESUME, D, BEST_REP, N_ITER, N_REP)    
+    
+    return RESULTS_REP, BEST_REP, AVERAGE_REP, WORST_REP, STATUS_PROCEDURE
```

### Comparing `META_TOOLBOX-2023.1/META_TOOLBOX/META_CO_LIBRARY.py` & `META_TOOLBOX-2023.2/META_TOOLBOX/META_CO_LIBRARY.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,221 +1,221 @@
-import numpy as np
-import pandas as pd
-
-def INITIAL_POPULATION_01(N_POP, D, X_L, X_U):
-    """ 
-    This function initializes the population randomically between the limits X_L and X_U.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/CO.html
-    """
-    
-    X_NEW = np.zeros((N_POP, D))
-
-    for I in range(N_POP):
-        for J in range(D):
-            RANDON_NUMBER = np.random.random()
-            X_NEW[I, J] = X_L[J] + (X_U[J] - X_L[J]) * RANDON_NUMBER
-    
-    return X_NEW
-
-def CHECK_INTERVAL_01(X_IOLD, X_L, X_U):
-    """
-    This function checks if a design variable is out of the limits established X_L and X_U.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/CO.html
-    """
-    
-    X_INEW = np.clip(X_IOLD, X_L, X_U)
-    
-    return X_INEW
-
-def FIT_VALUE(OF_VALUEI):
-    """ 
-    This function calculates the fitness of a value of the objective function.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/CO.html
-    """
-    # Positive OF
-    if OF_VALUEI >= 0:
-        FIT_VALUEI = 1 / (1 + OF_VALUEI)
-    # Negative OF
-    elif OF_VALUEI < 0:
-        FIT_VALUEI = 1 + abs(OF_VALUEI)
-    
-    return FIT_VALUEI
-
-def BEST_VALUES(X, OF, FIT, N_POP):
-    """ 
-    This function determines the best and worst particle. It also determines the average value (OF and FIT) of the population.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/CO.html
-    """
-    
-    # Best and worst ID in population
-    SORT_POSITIONS = np.argsort(OF.T)
-    BEST_POSITION = SORT_POSITIONS[0, 0]
-    WORST_POSITION = SORT_POSITIONS[0, N_POP - 1]
-
-    # Global best values
-    X_BEST = X[BEST_POSITION, :]
-    OF_BEST = OF[BEST_POSITION, 0]
-    FIT_BEST = FIT[BEST_POSITION, 0]
-    
-    # Global worst values
-    X_WORST = X[WORST_POSITION, :]
-    OF_WORST = OF[WORST_POSITION, 0]
-    FIT_WORST = FIT[WORST_POSITION, 0]
-    
-    # Average values
-    OF_AVERAGE = np.mean(OF)
-    FIT_AVERAGE = np.mean(FIT)
-
-    return BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE
-
-def PROGRESS_BAR(REP, TOTAL, PREFIX = 'Progress:', SUFFIX = 'Complete', DECIMALS = 1, LENGTH = 50, FILL = '█', PRINT_END = "\r"):
-    """
-    This function create terminal progress bar.
-    
-    Input:
-    REP        | Current iteration (required)                     | Integer
-    TOTAL      | Total iterations (required)                      | Integer
-    PREFIX     | Prefix string                                    | String
-    SUFFIX     | Suffix string                                    | String
-    DECIMALS   | Positive number of decimals in percent complete  | Integer
-    LENGTH     | Character length of bar                          | Integer
-    FILL       | Bar fill character                               | String
-    PRINT_END  | End character (e.g. "\r", "\r\n")                | String
-    
-    Output:
-    N/A
-    """
-    
-    # Progress bar
-    PERCENT = ("{0:." + str(DECIMALS) + "f}").format(100 * (REP / float(TOTAL)))
-    FILLED_LENGTH = int(LENGTH * REP // TOTAL)
-    BAR = FILL * FILLED_LENGTH + '-' * (LENGTH - FILLED_LENGTH)
-    print(f'\r{PREFIX} |{BAR}| {PERCENT}% {SUFFIX}', end = PRINT_END)
-    
-    # Print new line on complete
-    if REP == TOTAL: 
-        print()
-    
-    return
-
-def SUMMARY_ANALYSIS(BEST_REP, N_REP, N_ITER):
-    """ 
-    This function presents a written summary of the best simulation. 
-
-    Input:
-    BEST_REP         | Best population results by repetition                            | Py dictionary
-                     |   Dictionary tags                                                |
-                     |     'X_POSITION'    = Design variables by iteration              | Py Numpy array[N_ITER + 1 x D]
-                     |     'OF'            = Obj function value by iteration            | Py Numpy array[N_ITER + 1 x 1]
-                     |     'FIT'           = Fitness value by iteration                 | Py Numpy array[N_ITER + 1 x 1]
-                     |     '??_PARAMETERS' = Algorithm parametrs                        | Py Numpy array[N_ITER + 1 x 1]
-                     |     'NEOF'          = Number of objective function evaluations   | Py Numpy array[N_ITER + 1 x 1]
-                     |     'ID_PARTICLE'   = ID best particle by iteration              | Integer 
-    N_REP            | Number of repetitions                                            | Integer
-    N_ITER           | Number of iterations                                             | Integer
-
-    Output:
-    STATUS_PROCEDURE | Process repetition ID - from lowest OF value to highest OF value | Py list[N_REP]
-    """ 
-    
-    # Start reserved space for repetitions
-    OF_MINVALUES = []
-    
-    # Checking which is the best process 
-    for I_COUNT in range(N_REP):
-        ID = I_COUNT
-        OF_MIN = BEST_REP[ID]['OF'][N_ITER]
-        OF_MINVALUES.append(OF_MIN)
-    STATUS_PROCEDURE = np.argsort(OF_MINVALUES)    
-    
-    return STATUS_PROCEDURE
-
-def EXCEL_WRITER_ITERATION(NAME, D, DATASET):
-    """
-    This function create output Excel files by iteration.
-    
-    Input:
-    NAME       | Filename                                         | String
-    D          | Problem dimension                                | Integer
-    DATASET    | Best results I repetition                        | Py Numpy array
-    
-    Output:
-    Save xls file in current directory
-    """
-    
-    # Individual results
-    X = DATASET['X_POSITION']
-    COLUMNS = []
-    for I_COUNT in range(D):
-        COLUMNS_X = 'X_' + str(I_COUNT)
-        COLUMNS.append(COLUMNS_X)
-    DATA1 = pd.DataFrame(X, columns = COLUMNS)
-    OF = DATASET['OF']
-    DATA2 = pd.DataFrame(OF, columns = ['OF'])
-    FIT = DATASET['FIT']
-    DATA3 = pd.DataFrame(FIT, columns = ['FIT'])
-    NEOF = DATASET['NEOF']
-    DATA4 = pd.DataFrame(NEOF, columns = ['NEOF'])
-    FRAME = [DATA1, DATA2, DATA3, DATA4]
-    DATA = pd.concat(FRAME, axis = 1)
-    NAME += '.xlsx' 
-    print(NAME)
-    WRITER = pd.ExcelWriter(NAME, engine = 'xlsxwriter')
-    DATA.to_excel(WRITER, sheet_name = 'Sheet1')
-    WRITER.save()
-
-def EXCEL_PROCESS_RESUME(NAME, D, DATASET, N_ITER, N_REP):
-    """
-    This function create output Excel files complete process.
-
-    Input:
-    NAME       | Filename                                         | String
-    D          | Problem dimension                                | Integer
-    DATASET    | Best results I repetition                        | Py Numpy array
-    N_REP      | Number of repetitions                            | Integer
-    N_ITER     | Number of iterations                             | Integer
-
-    Output:
-    Save xls file in current directory
-    """
-    
-    # Resume process in arrays
-    X = np.zeros((N_REP, D))
-    OF = np.zeros((N_REP, 1))
-    FIT = np.zeros((N_REP, 1))
-    NEOF = np.zeros((N_REP, 1))
-    for REP in range(N_REP):
-        X_I = DATASET[REP]['X_POSITION'][N_ITER]
-        X[REP, :] = X_I
-        OF[REP, :] = DATASET[REP]['OF'][N_ITER]
-        FIT[REP, :] = DATASET[REP]['FIT'][N_ITER]
-        NEOF[REP, :] = DATASET[REP]['NEOF'][N_ITER]
-    
-    # Save output in Excel file
-    COLUMNS = []
-    for I in range(D):
-        COLUMNS_X = 'X_' + str(I)
-        COLUMNS.append(COLUMNS_X)
-    DATA1 = pd.DataFrame(X, columns = COLUMNS)
-    DATA2 = pd.DataFrame(OF, columns = ['OF'])
-    DATA3 = pd.DataFrame(FIT, columns = ['FIT'])
-    DATA4 = pd.DataFrame(NEOF, columns = ['NEOF'])
-    FRAME = [DATA1, DATA2, DATA3, DATA4]
-    DATA = pd.concat(FRAME, axis = 1)
-    NAME += '.xlsx' 
-    print(NAME)
-    WRITER = pd.ExcelWriter(NAME, engine = 'xlsxwriter')
-    DATA.to_excel(WRITER, sheet_name = 'Sheet1')
-    WRITER.save()
-
-def CONVERT_CONTINUOUS_DISCRETE(X, DATA_DISCRETE):
-    """
-    """
-    X_NEW = []
-    for I in range(len(X)):
-        AUX = round(X[I])
-        X_NEW.append(DATA_DISCRETE[I]['X'][AUX])
+import numpy as np
+import pandas as pd
+
+def INITIAL_POPULATION_01(N_POP, D, X_L, X_U):
+    """ 
+    This function initializes the population randomically between the limits X_L and X_U.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/CO.html
+    """
+    
+    X_NEW = np.zeros((N_POP, D))
+
+    for I in range(N_POP):
+        for J in range(D):
+            RANDON_NUMBER = np.random.random()
+            X_NEW[I, J] = X_L[J] + (X_U[J] - X_L[J]) * RANDON_NUMBER
+    
+    return X_NEW
+
+def CHECK_INTERVAL_01(X_IOLD, X_L, X_U):
+    """
+    This function checks if a design variable is out of the limits established X_L and X_U.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/CO.html
+    """
+    
+    X_INEW = np.clip(X_IOLD, X_L, X_U)
+    
+    return X_INEW
+
+def FIT_VALUE(OF_VALUEI):
+    """ 
+    This function calculates the fitness of a value of the objective function.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/CO.html
+    """
+    # Positive OF
+    if OF_VALUEI >= 0:
+        FIT_VALUEI = 1 / (1 + OF_VALUEI)
+    # Negative OF
+    elif OF_VALUEI < 0:
+        FIT_VALUEI = 1 + abs(OF_VALUEI)
+    
+    return FIT_VALUEI
+
+def BEST_VALUES(X, OF, FIT, N_POP):
+    """ 
+    This function determines the best and worst particle. It also determines the average value (OF and FIT) of the population.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/CO.html
+    """
+    
+    # Best and worst ID in population
+    SORT_POSITIONS = np.argsort(OF.T)
+    BEST_POSITION = SORT_POSITIONS[0, 0]
+    WORST_POSITION = SORT_POSITIONS[0, N_POP - 1]
+
+    # Global best values
+    X_BEST = X[BEST_POSITION, :]
+    OF_BEST = OF[BEST_POSITION, 0]
+    FIT_BEST = FIT[BEST_POSITION, 0]
+    
+    # Global worst values
+    X_WORST = X[WORST_POSITION, :]
+    OF_WORST = OF[WORST_POSITION, 0]
+    FIT_WORST = FIT[WORST_POSITION, 0]
+    
+    # Average values
+    OF_AVERAGE = np.mean(OF)
+    FIT_AVERAGE = np.mean(FIT)
+
+    return BEST_POSITION, WORST_POSITION, X_BEST, X_WORST, OF_BEST, OF_WORST, FIT_BEST, FIT_WORST, OF_AVERAGE, FIT_AVERAGE
+
+def PROGRESS_BAR(REP, TOTAL, PREFIX = 'Progress:', SUFFIX = 'Complete', DECIMALS = 1, LENGTH = 50, FILL = '█', PRINT_END = "\r"):
+    """
+    This function create terminal progress bar.
+    
+    Input:
+    REP        | Current iteration (required)                     | Integer
+    TOTAL      | Total iterations (required)                      | Integer
+    PREFIX     | Prefix string                                    | String
+    SUFFIX     | Suffix string                                    | String
+    DECIMALS   | Positive number of decimals in percent complete  | Integer
+    LENGTH     | Character length of bar                          | Integer
+    FILL       | Bar fill character                               | String
+    PRINT_END  | End character (e.g. "\r", "\r\n")                | String
+    
+    Output:
+    N/A
+    """
+    
+    # Progress bar
+    PERCENT = ("{0:." + str(DECIMALS) + "f}").format(100 * (REP / float(TOTAL)))
+    FILLED_LENGTH = int(LENGTH * REP // TOTAL)
+    BAR = FILL * FILLED_LENGTH + '-' * (LENGTH - FILLED_LENGTH)
+    print(f'\r{PREFIX} |{BAR}| {PERCENT}% {SUFFIX}', end = PRINT_END)
+    
+    # Print new line on complete
+    if REP == TOTAL: 
+        print()
+    
+    return
+
+def SUMMARY_ANALYSIS(BEST_REP, N_REP, N_ITER):
+    """ 
+    This function presents a written summary of the best simulation. 
+
+    Input:
+    BEST_REP         | Best population results by repetition                            | Py dictionary
+                     |   Dictionary tags                                                |
+                     |     'X_POSITION'    = Design variables by iteration              | Py Numpy array[N_ITER + 1 x D]
+                     |     'OF'            = Obj function value by iteration            | Py Numpy array[N_ITER + 1 x 1]
+                     |     'FIT'           = Fitness value by iteration                 | Py Numpy array[N_ITER + 1 x 1]
+                     |     '??_PARAMETERS' = Algorithm parametrs                        | Py Numpy array[N_ITER + 1 x 1]
+                     |     'NEOF'          = Number of objective function evaluations   | Py Numpy array[N_ITER + 1 x 1]
+                     |     'ID_PARTICLE'   = ID best particle by iteration              | Integer 
+    N_REP            | Number of repetitions                                            | Integer
+    N_ITER           | Number of iterations                                             | Integer
+
+    Output:
+    STATUS_PROCEDURE | Process repetition ID - from lowest OF value to highest OF value | Py list[N_REP]
+    """ 
+    
+    # Start reserved space for repetitions
+    OF_MINVALUES = []
+    
+    # Checking which is the best process 
+    for I_COUNT in range(N_REP):
+        ID = I_COUNT
+        OF_MIN = BEST_REP[ID]['OF'][N_ITER]
+        OF_MINVALUES.append(OF_MIN)
+    STATUS_PROCEDURE = np.argsort(OF_MINVALUES)    
+    
+    return STATUS_PROCEDURE
+
+def EXCEL_WRITER_ITERATION(NAME, D, DATASET):
+    """
+    This function create output Excel files by iteration.
+    
+    Input:
+    NAME       | Filename                                         | String
+    D          | Problem dimension                                | Integer
+    DATASET    | Best results I repetition                        | Py Numpy array
+    
+    Output:
+    Save xls file in current directory
+    """
+    
+    # Individual results
+    X = DATASET['X_POSITION']
+    COLUMNS = []
+    for I_COUNT in range(D):
+        COLUMNS_X = 'X_' + str(I_COUNT)
+        COLUMNS.append(COLUMNS_X)
+    DATA1 = pd.DataFrame(X, columns = COLUMNS)
+    OF = DATASET['OF']
+    DATA2 = pd.DataFrame(OF, columns = ['OF'])
+    FIT = DATASET['FIT']
+    DATA3 = pd.DataFrame(FIT, columns = ['FIT'])
+    NEOF = DATASET['NEOF']
+    DATA4 = pd.DataFrame(NEOF, columns = ['NEOF'])
+    FRAME = [DATA1, DATA2, DATA3, DATA4]
+    DATA = pd.concat(FRAME, axis = 1)
+    NAME += '.xlsx' 
+    print(NAME)
+    WRITER = pd.ExcelWriter(NAME, engine = 'xlsxwriter')
+    DATA.to_excel(WRITER, sheet_name = 'Sheet1')
+    WRITER.close()
+
+def EXCEL_PROCESS_RESUME(NAME, D, DATASET, N_ITER, N_REP):
+    """
+    This function create output Excel files complete process.
+
+    Input:
+    NAME       | Filename                                         | String
+    D          | Problem dimension                                | Integer
+    DATASET    | Best results I repetition                        | Py Numpy array
+    N_REP      | Number of repetitions                            | Integer
+    N_ITER     | Number of iterations                             | Integer
+
+    Output:
+    Save xls file in current directory
+    """
+    
+    # Resume process in arrays
+    X = np.zeros((N_REP, D))
+    OF = np.zeros((N_REP, 1))
+    FIT = np.zeros((N_REP, 1))
+    NEOF = np.zeros((N_REP, 1))
+    for REP in range(N_REP):
+        X_I = DATASET[REP]['X_POSITION'][N_ITER]
+        X[REP, :] = X_I
+        OF[REP, :] = DATASET[REP]['OF'][N_ITER]
+        FIT[REP, :] = DATASET[REP]['FIT'][N_ITER]
+        NEOF[REP, :] = DATASET[REP]['NEOF'][N_ITER]
+    
+    # Save output in Excel file
+    COLUMNS = []
+    for I in range(D):
+        COLUMNS_X = 'X_' + str(I)
+        COLUMNS.append(COLUMNS_X)
+    DATA1 = pd.DataFrame(X, columns = COLUMNS)
+    DATA2 = pd.DataFrame(OF, columns = ['OF'])
+    DATA3 = pd.DataFrame(FIT, columns = ['FIT'])
+    DATA4 = pd.DataFrame(NEOF, columns = ['NEOF'])
+    FRAME = [DATA1, DATA2, DATA3, DATA4]
+    DATA = pd.concat(FRAME, axis = 1)
+    NAME += '.xlsx' 
+    print(NAME)
+    WRITER = pd.ExcelWriter(NAME, engine = 'xlsxwriter')
+    DATA.to_excel(WRITER, sheet_name = 'Sheet1')
+    WRITER.close()
+
+def CONVERT_CONTINUOUS_DISCRETE(X, DATA_DISCRETE):
+    """
+    """
+    X_NEW = []
+    for I in range(len(X)):
+        AUX = round(X[I])
+        X_NEW.append(DATA_DISCRETE[I]['X'][AUX])
     return X_NEW
```

### Comparing `META_TOOLBOX-2023.1/META_TOOLBOX/META_FA_LIBRARY.py` & `META_TOOLBOX-2023.2/META_TOOLBOX/META_FA_LIBRARY.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,189 +1,306 @@
-import numpy as np
-import META_TOOLBOX.META_CO_LIBRARY as META_CL
-
-# CHAOTIC SEARCH
-def CHAOTIC_SEARCH(OF_FUNCTION, ITER, X_BEST, OF_BEST, FIT_BEST, N_CHAOTICSEARCHS, ALPHA_CHAOTIC, D, N_ITER, X_L, X_U, NULL_DIC):
-    # INITIALIZATION VARIABLES
-    K = N_CHAOTICSEARCHS
-    CH = []
-    X_BESTNEW = X_BEST
-    OF_BESTNEW = OF_BEST
-    FIT_BESTNEW = FIT_BEST
-    # CSI UPDATE
-    CSI = (N_ITER - ITER + 1) / N_ITER
-    # CHAOTIC SEARCHS
-    for I_COUNT in range(0, K):
-        CH_XBEST = np.zeros((1, D))
-        X_BESTTEMPORARY = np.zeros((1, D))
-        if I_COUNT == 0:
-            # CHAOTIC UPDATE
-            CH.append(np.random.random())
-        else:
-            # CHAOTIC UPDATE POSITION, OF AND FIT
-            CH.append(ALPHA_CHAOTIC * CH[I_COUNT - 1] * (1 - CH[I_COUNT - 1]))
-        # CREATING THE CHAOTIC POSITION
-        for J_COUNT in range(D): 
-            CH_XBEST[0, J_COUNT] = X_L[J_COUNT] + (X_U[J_COUNT] - X_L[J_COUNT]) * CH[I_COUNT]
-            # print('aqui', type(X_BESTNEW), X_BESTNEW)
-            X_BESTTEMPORARY[0, J_COUNT] = (1 - CSI) * X_BESTNEW[J_COUNT] + CSI * CH_XBEST[0, J_COUNT]
-        X_BESTTEMPORARY[0, :] = META_CL.CHECK_INTERVAL_01(X_BESTTEMPORARY[0, :], X_L, X_U) 
-        OF_BESTTEMPORARY = OF_FUNCTION(X_BESTTEMPORARY[0, :], NULL_DIC)
-        FIT_BESTTEMPORARY = META_CL.FIT_VALUE(OF_BESTTEMPORARY)
-        # STORING BEST VALUE
-        if FIT_BESTTEMPORARY > FIT_BEST:
-            X_BESTNEW = X_BESTTEMPORARY[0, :]
-            OF_BESTNEW = OF_BESTTEMPORARY
-            FIT_BESTNEW = FIT_BESTTEMPORARY
-    return X_BESTNEW, OF_BESTNEW, FIT_BESTNEW
-
-# CALCULATION OF THE DISCRIMINATING FACTOR OF THE MALE AND FEMALE FIREFLIES POPULATION
-def DISCRIMINANT_FACTOR_MALE_MOVIMENT(FIT_XI, FIT_YK):
-    """ COMENTÁRIO NATIVO VOU FAZER"""
-    # COMPARISON OF FIREFLY BRIGHTNESS
-    if FIT_XI > FIT_YK:
-        D_1 = 1
-    else:
-        D_1 = -1
-    return D_1
-
-# DETERMINAÇÃO DO FATOR DE ATRATIVIDADE BETA
-def ATTRACTIVENESS_FIREFLY_PARAMETER(BETA_0, GAMMA, X_I, X_J, D):
-    """
-    This function calculates distance between X_I and X_J fireflies.
-
-    Input:
-    BETA_0  | Attractiveness at r = 0                             | Float
-    GAMMA   | Light absorption coefficient  1 / (X_U - X_L) ** M  | Py list[D]
-    X_I     | I Firefly                                           | Py list[D]
-    X_J     | J Firefly                                           | Py list[D]
-    D       | Problem dimension                                   | Integer
-
-    Output:
-    BETA    | Attractiveness                                      | Py list[D]
-    """
-    AUX = 0
-    
-    # Firefly distance
-    for I_COUNT in range(D):
-        AUX += (X_I[I_COUNT] - X_J[I_COUNT]) ** 2
-    R_IJ = np.sqrt(AUX)
-    
-    # Beta attractiveness
-    BETA = []
-    for J_COUNT in range(D):
-        BETA.append(BETA_0 * np.exp(- GAMMA[J_COUNT] * R_IJ))
-    
-    return BETA
-
-# MOVIMENTO DE UM VAGALUME TRADICIONAL
-def FIREFLY_MOVEMENT(OF_FUNCTION, X_T0I, X_J, BETA, ALPHA, D, X_L, X_U, NULL_DIC):
-    """
-    This function creates a new solution using FA movement algorithm.
-
-    Input:
-    OF_FUNCTION  | External def user input this function in arguments       | Py function
-    X_T0I        | Design variable I particle before movement               | Py list[D]
-    X_J          | J Firefly                                                | Py list[D]
-    BETA         | Attractiveness                                           | Py list[D]
-    ALPHA        | Randomic factor                                          | Float
-    D            | Problem dimension                                        | Integer
-    X_L          | Lower limit design variables                             | Py list[D]
-    X_U          | Upper limit design variables                             | Py list[D]
-    NULL_DIC     | Empty variable for the user to use in the obj. function  | ? 
-    
-    Output:
-    X_T1I        | Design variable I particle after movement                | Py list[D]
-    OF_T1I       | Objective function X_T1I (new particle)                  | Float
-    FIT_T1I      | Fitness X_T1I (new particle)                             | Float
-    NEOF         | Number of objective function evaluations                 | Integer
-    """
-    # Start internal variables
-    X_T1I = []
-    OF_T1I = 0
-    FIT_T1I = 0
-    for I_COUNT in range(D):
-        EPSILON_I = np.random.random() - 0.50
-        NEW_VALUE = X_T0I[I_COUNT] + BETA[I_COUNT] * (X_J[I_COUNT] - X_T0I[I_COUNT]) + ALPHA * EPSILON_I
-        X_T1I.append(NEW_VALUE) 
-    # Check boundes
-    X_T1I = META_CL.CHECK_INTERVAL_01(X_T1I, X_L, X_U) 
-    # Evaluation of the objective function and fitness
-    OF_T1I = OF_FUNCTION(X_T1I, NULL_DIC)
-    FIT_T1I = META_CL.FIT_VALUE(OF_T1I)
-    NEOF = 1
-    return X_T1I, OF_T1I, FIT_T1I, NEOF
-
-# MALE FIREFLY MOVEMENT
-def MALE_FIREFLY_MOVEMENT(OF_FUNCTION, X_MALECURRENTI, FIT_MALECURRENTI, Y_FEMALECURRENTK, FIT_FEMALECURRENTK, Y_FEMALECURRENTJ, FIT_FEMALECURRENTJ, BETA_0, GAMMA, D, X_L, X_U, NULL_DIC):
-    """ COMENTÁRIO NATIVO VOU FAZER"""
-    # INITIALIZATION VARIABLES
-    SECOND_TERM = []
-    THIRD_TERM = []
-    X_MALENEWI = []
-    # DISCRIMINANT D FACTOR
-    D_1 = DISCRIMINANT_FACTOR_MALE_MOVIMENT(FIT_MALECURRENTI, FIT_FEMALECURRENTK)
-    D_2 = DISCRIMINANT_FACTOR_MALE_MOVIMENT(FIT_MALECURRENTI, FIT_FEMALECURRENTJ)
-    # ATTRACTIVENESS AMONG FIREFLIES
-    BETA_1 = ATTRACTIVENESS_FIREFLY_PARAMETER(BETA_0, GAMMA, X_MALECURRENTI, Y_FEMALECURRENTK, D)
-    BETA_2 = ATTRACTIVENESS_FIREFLY_PARAMETER(BETA_0, GAMMA, X_MALECURRENTI, Y_FEMALECURRENTJ, D)
-    # LAMBDA AND MU RANDOM PARAMETERS
-    LAMBDA = np.random.random()
-    MU = np.random.random()
-    for I_COUNT in range(D):
-        SECOND_TERM.append(D_1 * BETA_1[I_COUNT] * LAMBDA * (Y_FEMALECURRENTK[I_COUNT] - X_MALECURRENTI[I_COUNT]))
-        THIRD_TERM.append(D_2 * BETA_2[I_COUNT] * MU * (Y_FEMALECURRENTJ[I_COUNT] - X_MALECURRENTI[I_COUNT]))
-    # UPDATE FEMALE POSITION, OF AND FIT
-    for J_COUNT in range(D):
-        X_MALENEWI.append(X_MALECURRENTI[J_COUNT] + SECOND_TERM[J_COUNT] + THIRD_TERM[J_COUNT])
-    X_MALENEWI = META_CL.CHECK_INTERVAL_01(X_MALENEWI, X_L, X_U) 
-    OF_MALENEWI = OF_FUNCTION(X_MALENEWI, NULL_DIC)
-    FIT_MALENEWI = META_CL.FIT_VALUE(OF_MALENEWI)
-    return X_MALENEWI, OF_MALENEWI, FIT_MALENEWI
-
-# FEMALE FIREFLY MOVEMENT
-def FEMALE_FIREFLY_MOVEMENT(OF_FUNCTION, Y_FEMALECURRENTI, X_MALEBEST, FIT_MALEBEST, BETA_0, GAMMA, D, X_L, X_U, NULL_DIC):
-    """ COMENTÁRIO NATIVO VOU FAZER"""
-    # INITIALIZATION VARIABLES
-    Y_FEMALENEWI = []
-    # ATTRACTIVENESS AMONG FIREFLIES (Y_FEMALE AND X_BEST)
-    BETA = ATTRACTIVENESS_FIREFLY_PARAMETER(BETA_0, GAMMA, Y_FEMALECURRENTI, X_MALEBEST, D)
-    # PHI RANDOM PARAMETER
-    PHI = np.random.random()
-    # UPDATE FEMALE POSITION, OF AND FIT
-    for I_COUNT in range(D):
-        Y_FEMALENEWI.append(Y_FEMALECURRENTI[I_COUNT] + BETA[I_COUNT] * PHI * (X_MALEBEST[I_COUNT] - Y_FEMALECURRENTI[I_COUNT]))
-    Y_FEMALENEWI = META_CL.CHECK_INTERVAL(Y_FEMALENEWI, X_L, X_U)
-    OF_FEMALENEWI = OF_FUNCTION(Y_FEMALENEWI, NULL_DIC)
-    FIT_FEMALENEWI = META_CL.FIT_VALUE(OF_FEMALENEWI)
-    return Y_FEMALENEWI, OF_FEMALENEWI, FIT_FEMALENEWI
-
-# FATOR DE ABSORÇÃO DE LUZ GAMMA
-def GAMMA_ASSEMBLY(X_L, X_U, D, M):
-    """
-    This function calculates the light absorption coefficient.
-
-    Input:
-    X_L    | Lower limit design variables                        | Py list[D]
-    X_U    | Upper limit design variables                        | Py list[D]
-    D      | Problem dimension                                   | Integer
-    M      | Exponent value in distance                          | Float  
-
-    Output:
-    GAMMA  | Light absorption coefficient  1 / (X_U - X_L) ** M  | Py list[D] 
-    """
-    
-    GAMMA = []
-    for I_COUNT in range(D):
-        DISTANCE = X_U[0] - X_L[0]
-        GAMMA.append(1 / DISTANCE ** M)
-    
-    return GAMMA
-
-#   /$$$$$$  /$$$$$$$  /$$$$$$$$ /$$$$$$$$       /$$$$$$$$ /$$$$$$$$  /$$$$$$  /$$   /$$ /$$   /$$  /$$$$$$  /$$        /$$$$$$   /$$$$$$  /$$$$$$ /$$$$$$$$  /$$$$$$ 
-#  /$$__  $$| $$__  $$| $$_____/| $$_____/      |__  $$__/| $$_____/ /$$__  $$| $$  | $$| $$$ | $$ /$$__  $$| $$       /$$__  $$ /$$__  $$|_  $$_/| $$_____/ /$$__  $$
-# | $$  \__/| $$  \ $$| $$      | $$               | $$   | $$      | $$  \__/| $$  | $$| $$$$| $$| $$  \ $$| $$      | $$  \ $$| $$  \__/  | $$  | $$      | $$  \__/
-# | $$ /$$$$| $$$$$$$/| $$$$$   | $$$$$            | $$   | $$$$$   | $$      | $$$$$$$$| $$ $$ $$| $$  | $$| $$      | $$  | $$| $$ /$$$$  | $$  | $$$$$   |  $$$$$$ 
-# | $$|_  $$| $$____/ | $$__/   | $$__/            | $$   | $$__/   | $$      | $$__  $$| $$  $$$$| $$  | $$| $$      | $$  | $$| $$|_  $$  | $$  | $$__/    \____  $$
-# | $$  \ $$| $$      | $$      | $$               | $$   | $$      | $$    $$| $$  | $$| $$\  $$$| $$  | $$| $$      | $$  | $$| $$  \ $$  | $$  | $$       /$$  \ $$
-# |  $$$$$$/| $$      | $$$$$$$$| $$$$$$$$         | $$   | $$$$$$$$|  $$$$$$/| $$  | $$| $$ \  $$|  $$$$$$/| $$$$$$$$|  $$$$$$/|  $$$$$$/ /$$$$$$| $$$$$$$$|  $$$$$$/
+import numpy as np
+import META_TOOLBOX.META_CO_LIBRARY as META_CL
+
+# CHAOTIC SEARCH
+def CHAOTIC_SEARCH(OF_FUNCTION, ITER, X_BEST, OF_BEST, FIT_BEST, N_CHAOTICSEARCHS, ALPHA_CHAOTIC, D, N_ITER, X_L, X_U, NULL_DIC):
+    # INITIALIZATION VARIABLES
+    K = N_CHAOTICSEARCHS
+    CH = []
+    X_BESTNEW = X_BEST
+    OF_BESTNEW = OF_BEST
+    FIT_BESTNEW = FIT_BEST
+    # CSI UPDATE
+    CSI = (N_ITER - ITER + 1) / N_ITER
+    # CHAOTIC SEARCHS
+    for I_COUNT in range(0, K):
+        CH_XBEST = np.zeros((1, D))
+        X_BESTTEMPORARY = np.zeros((1, D))
+        if I_COUNT == 0:
+            # CHAOTIC UPDATE
+            CH.append(np.random.random())
+        else:
+            # CHAOTIC UPDATE POSITION, OF AND FIT
+            CH.append(ALPHA_CHAOTIC * CH[I_COUNT - 1] * (1 - CH[I_COUNT - 1]))
+        # CREATING THE CHAOTIC POSITION
+        for J_COUNT in range(D): 
+            CH_XBEST[0, J_COUNT] = X_L[J_COUNT] + (X_U[J_COUNT] - X_L[J_COUNT]) * CH[I_COUNT]
+            # print('aqui', type(X_BESTNEW), X_BESTNEW)
+            X_BESTTEMPORARY[0, J_COUNT] = (1 - CSI) * X_BESTNEW[J_COUNT] + CSI * CH_XBEST[0, J_COUNT]
+        X_BESTTEMPORARY[0, :] = META_CL.CHECK_INTERVAL_01(X_BESTTEMPORARY[0, :], X_L, X_U) 
+        OF_BESTTEMPORARY = OF_FUNCTION(X_BESTTEMPORARY[0, :], NULL_DIC)
+        FIT_BESTTEMPORARY = META_CL.FIT_VALUE(OF_BESTTEMPORARY)
+        # STORING BEST VALUE
+        if FIT_BESTTEMPORARY > FIT_BEST:
+            X_BESTNEW = X_BESTTEMPORARY[0, :]
+            OF_BESTNEW = OF_BESTTEMPORARY
+            FIT_BESTNEW = FIT_BESTTEMPORARY
+    return X_BESTNEW, OF_BESTNEW, FIT_BESTNEW
+
+# CALCULATION OF THE DISCRIMINATING FACTOR OF THE MALE AND FEMALE FIREFLIES POPULATION
+def DISCRIMINANT_FACTOR_MALE_MOVIMENT(FIT_XI, FIT_YK):
+    """ COMENTÁRIO NATIVO VOU FAZER"""
+    # COMPARISON OF FIREFLY BRIGHTNESS
+    if FIT_XI > FIT_YK:
+        D_1 = 1
+    else:
+        D_1 = -1
+    return D_1
+
+# DETERMINAÇÃO DO FATOR DE ATRATIVIDADE BETA
+def ATTRACTIVENESS_FIREFLY_PARAMETER(BETA_0, GAMMA, X_I, X_J, D):
+    """
+    This function calculates distance between X_I and X_J fireflies.
+
+    Input:
+    BETA_0  | Attractiveness at r = 0                             | Float
+    GAMMA   | Light absorption coefficient  1 / (X_U - X_L) ** M  | Py list[D]
+    X_I     | I Firefly                                           | Py list[D]
+    X_J     | J Firefly                                           | Py list[D]
+    D       | Problem dimension                                   | Integer
+
+    Output:
+    BETA    | Attractiveness                                      | Py list[D]
+    """
+    AUX = 0
+    
+    # Firefly distance
+    for I_COUNT in range(D):
+        AUX += (X_I[I_COUNT] - X_J[I_COUNT]) ** 2
+    R_IJ = np.sqrt(AUX)
+    
+    # Beta attractiveness
+    BETA = []
+    for J_COUNT in range(D):
+        BETA.append(BETA_0 * np.exp(- GAMMA[J_COUNT] * R_IJ))
+    
+    return BETA
+
+# MOVIMENTO DE UM VAGALUME TRADICIONAL
+def FIREFLY_MOVEMENT(OF_FUNCTION, X_T0I, X_J, BETA, ALPHA, SCALING, D, X_L, X_U, NULL_DIC):
+    """
+    This function creates a new solution using FA movement algorithm.
+
+    Input:
+    OF_FUNCTION  | External def user input this function in arguments       | Py function
+    X_T0I        | Design variable I particle before movement               | Py list[D]
+    X_J          | J Firefly                                                | Py list[D]
+    BETA         | Attractiveness                                           | Py list[D]
+    ALPHA        | Randomic factor                                          | Float
+    D            | Problem dimension                                        | Integer
+    X_L          | Lower limit design variables                             | Py list[D]
+    X_U          | Upper limit design variables                             | Py list[D]
+    NULL_DIC     | Empty variable for the user to use in the obj. function  | ? 
+    
+    Output:
+    X_T1I        | Design variable I particle after movement                | Py list[D]
+    OF_T1I       | Objective function X_T1I (new particle)                  | Float
+    FIT_T1I      | Fitness X_T1I (new particle)                             | Float
+    NEOF         | Number of objective function evaluations                 | Integer
+    """
+    # Start internal variables
+    X_T1I = []
+    OF_T1I = 0
+    FIT_T1I = 0
+    for I_COUNT in range(D):
+        EPSILON_I = np.random.random() - 0.50
+        if SCALING:
+            S_D = X_U[I_COUNT] - X_L[I_COUNT]
+        else:
+            S_D = 1
+        NEW_VALUE = X_T0I[I_COUNT] + BETA[I_COUNT] * (X_J[I_COUNT] - X_T0I[I_COUNT]) + ALPHA * S_D * EPSILON_I
+        X_T1I.append(NEW_VALUE) 
+    # Check boundes
+    X_T1I = META_CL.CHECK_INTERVAL_01(X_T1I, X_L, X_U) 
+    # Evaluation of the objective function and fitness
+    OF_T1I = OF_FUNCTION(X_T1I, NULL_DIC)
+    FIT_T1I = META_CL.FIT_VALUE(OF_T1I)
+    NEOF = 1
+    return X_T1I, OF_T1I, FIT_T1I, NEOF
+
+# MALE FIREFLY MOVEMENT
+def MALE_FIREFLY_MOVEMENT(OF_FUNCTION, X_MALECURRENTI, FIT_MALECURRENTI, Y_FEMALECURRENTK, FIT_FEMALECURRENTK, Y_FEMALECURRENTJ, FIT_FEMALECURRENTJ, BETA_0, GAMMA, D, X_L, X_U, NULL_DIC):
+    """ COMENTÁRIO NATIVO VOU FAZER"""
+    # INITIALIZATION VARIABLES
+    SECOND_TERM = []
+    THIRD_TERM = []
+    X_MALENEWI = []
+    # DISCRIMINANT D FACTOR
+    D_1 = DISCRIMINANT_FACTOR_MALE_MOVIMENT(FIT_MALECURRENTI, FIT_FEMALECURRENTK)
+    D_2 = DISCRIMINANT_FACTOR_MALE_MOVIMENT(FIT_MALECURRENTI, FIT_FEMALECURRENTJ)
+    # ATTRACTIVENESS AMONG FIREFLIES
+    BETA_1 = ATTRACTIVENESS_FIREFLY_PARAMETER(BETA_0, GAMMA, X_MALECURRENTI, Y_FEMALECURRENTK, D)
+    BETA_2 = ATTRACTIVENESS_FIREFLY_PARAMETER(BETA_0, GAMMA, X_MALECURRENTI, Y_FEMALECURRENTJ, D)
+    # LAMBDA AND MU RANDOM PARAMETERS
+    LAMBDA = np.random.random()
+    MU = np.random.random()
+    for I_COUNT in range(D):
+        SECOND_TERM.append(D_1 * BETA_1[I_COUNT] * LAMBDA * (Y_FEMALECURRENTK[I_COUNT] - X_MALECURRENTI[I_COUNT]))
+        THIRD_TERM.append(D_2 * BETA_2[I_COUNT] * MU * (Y_FEMALECURRENTJ[I_COUNT] - X_MALECURRENTI[I_COUNT]))
+    # UPDATE FEMALE POSITION, OF AND FIT
+    for J_COUNT in range(D):
+        X_MALENEWI.append(X_MALECURRENTI[J_COUNT] + SECOND_TERM[J_COUNT] + THIRD_TERM[J_COUNT])
+    X_MALENEWI = META_CL.CHECK_INTERVAL_01(X_MALENEWI, X_L, X_U) 
+    OF_MALENEWI = OF_FUNCTION(X_MALENEWI, NULL_DIC)
+    FIT_MALENEWI = META_CL.FIT_VALUE(OF_MALENEWI)
+    return X_MALENEWI, OF_MALENEWI, FIT_MALENEWI
+
+# FEMALE FIREFLY MOVEMENT
+def FEMALE_FIREFLY_MOVEMENT(OF_FUNCTION, Y_FEMALECURRENTI, X_MALEBEST, FIT_MALEBEST, BETA_0, GAMMA, D, X_L, X_U, NULL_DIC):
+    """ COMENTÁRIO NATIVO VOU FAZER"""
+    # INITIALIZATION VARIABLES
+    Y_FEMALENEWI = []
+    # ATTRACTIVENESS AMONG FIREFLIES (Y_FEMALE AND X_BEST)
+    BETA = ATTRACTIVENESS_FIREFLY_PARAMETER(BETA_0, GAMMA, Y_FEMALECURRENTI, X_MALEBEST, D)
+    # PHI RANDOM PARAMETER
+    PHI = np.random.random()
+    # UPDATE FEMALE POSITION, OF AND FIT
+    for I_COUNT in range(D):
+        Y_FEMALENEWI.append(Y_FEMALECURRENTI[I_COUNT] + BETA[I_COUNT] * PHI * (X_MALEBEST[I_COUNT] - Y_FEMALECURRENTI[I_COUNT]))
+    Y_FEMALENEWI = META_CL.CHECK_INTERVAL(Y_FEMALENEWI, X_L, X_U)
+    OF_FEMALENEWI = OF_FUNCTION(Y_FEMALENEWI, NULL_DIC)
+    FIT_FEMALENEWI = META_CL.FIT_VALUE(OF_FEMALENEWI)
+    return Y_FEMALENEWI, OF_FEMALENEWI, FIT_FEMALENEWI
+
+# FATOR DE ABSORÇÃO DE LUZ GAMMA
+def GAMMA_ASSEMBLY(X_L, X_U, D, M):
+    """
+    This function calculates the light absorption coefficient.
+
+    Input:
+    X_L    | Lower limit design variables                        | Py list[D]
+    X_U    | Upper limit design variables                        | Py list[D]
+    D      | Problem dimension                                   | Integer
+    M      | Exponent value in distance                          | Float  
+
+    Output:
+    GAMMA  | Light absorption coefficient  1 / (X_U - X_L) ** M  | Py list[D] 
+    """
+    
+    GAMMA = []
+    for I_COUNT in range(D):
+        DISTANCE = X_U[0] - X_L[0]
+        GAMMA.append(1 / DISTANCE ** M)
+    
+    return GAMMA
+
+def GDFA_MALE_MOVEMENT(OF_FUNCTION, X_T0I, Y_T0J, Y_T0K, GAMMA, BETA_0, D, X_L, X_U, NULL_DIC):
+    """
+    This function creates a new solution using FA movement algorithm.
+
+    Input:
+    OF_FUNCTION  | External def user input this function in arguments       | Py function
+    X_T0I        | Design variable I particle before movement               | Py list[D]
+    X_J          | J Firefly                                                | Py list[D]
+    BETA         | Attractiveness                                           | Py list[D]
+    ALPHA        | Randomic factor                                          | Float
+    D            | Problem dimension                                        | Integer
+    X_L          | Lower limit design variables                             | Py list[D]
+    X_U          | Upper limit design variables                             | Py list[D]
+    NULL_DIC     | Empty variable for the user to use in the obj. function  | ? 
+    
+    Output:
+    X_T1I        | Design variable I particle after movement                | Py list[D]
+    OF_T1I       | Objective function X_T1I (new particle)                  | Float
+    FIT_T1I      | Fitness X_T1I (new particle)                             | Float
+    NEOF         | Number of objective function evaluations                 | Integer
+    """
+
+    # Start internal variables
+    X_T1I = []
+    OF_T1I = 0
+    FIT_T1I = 0
+    BETA_J = ATTRACTIVENESS_FIREFLY_PARAMETER(BETA_0, GAMMA, X_T0I, Y_T0J, D)
+    BETA_K = ATTRACTIVENESS_FIREFLY_PARAMETER(BETA_0, GAMMA, X_T0I, Y_T0K, D)
+    
+    #D_1 
+    if Y_T0J < X_T0I:
+        D_1 = 1
+    else:
+        D_1 = -1
+    #D_2
+    if Y_T0K < X_T0I:
+        D_2 = 1
+    else:
+        D_2 = -1
+
+    for I_COUNT in range(D):
+        LAMBDA = np.random.random()
+        MICRO = np.random.random()
+        NEW_VALUE = X_T0I[I_COUNT] + D_1 * BETA_J[I_COUNT] * LAMBDA * (Y_T0J[I_COUNT] - X_T0I[I_COUNT])   
+        AUX_VALUE =  D_2 * BETA_K[I_COUNT] * MICRO * (Y_T0K[I_COUNT] - X_T0I[I_COUNT])    
+        NEW_VALUE += AUX_VALUE
+        X_T1I.append(NEW_VALUE) 
+    # Check boundes
+    X_T1I = META_CL.CHECK_INTERVAL_01(X_T1I, X_L, X_U) 
+    # Evaluation of the objective function and fitness
+    OF_T1I = OF_FUNCTION(X_T1I, NULL_DIC)
+    FIT_T1I = META_CL.FIT_VALUE(OF_T1I)
+    NEOF = 1
+    return X_T1I, OF_T1I, FIT_T1I, NEOF
+def GDFA_FEMALE_MOVEMENT(OF_FUNCTION, X_T0I, Y_T0J, Y_T0K, GAMMA, BETA_0, D, X_L, X_U, NULL_DIC):
+    """
+    This function creates a new solution using FA movement algorithm.
+
+    Input:
+    OF_FUNCTION  | External def user input this function in arguments       | Py function
+    X_T0I        | Design variable I particle before movement               | Py list[D]
+    X_J          | J Firefly                                                | Py list[D]
+    BETA         | Attractiveness                                           | Py list[D]
+    ALPHA        | Randomic factor                                          | Float
+    D            | Problem dimension                                        | Integer
+    X_L          | Lower limit design variables                             | Py list[D]
+    X_U          | Upper limit design variables                             | Py list[D]
+    NULL_DIC     | Empty variable for the user to use in the obj. function  | ? 
+    
+    Output:
+    X_T1I        | Design variable I particle after movement                | Py list[D]
+    OF_T1I       | Objective function X_T1I (new particle)                  | Float
+    FIT_T1I      | Fitness X_T1I (new particle)                             | Float
+    NEOF         | Number of objective function evaluations                 | Integer
+    """
+
+    # Start internal variables
+    X_T1I = []
+    OF_T1I = 0
+    FIT_T1I = 0
+    BETA_J = ATTRACTIVENESS_FIREFLY_PARAMETER(BETA_0, GAMMA, X_T0I, Y_T0J, D)
+    BETA_K = ATTRACTIVENESS_FIREFLY_PARAMETER(BETA_0, GAMMA, X_T0I, Y_T0K, D)
+    
+    #TENHO QUE MEXER AINDA
+    #D_1 
+    if Y_T0J < X_T0I:
+        D_1 = 1
+    else:
+        D_1 = -1
+    #D_2
+    if Y_T0K < X_T0I:
+        D_2 = 1
+    else:
+        D_2 = -1
+
+    for I_COUNT in range(D):
+        LAMBDA = np.random.random()
+        MICRO = np.random.random()
+        NEW_VALUE = X_T0I[I_COUNT] + D_1 * BETA_J[I_COUNT] * LAMBDA * (Y_T0J[I_COUNT] - X_T0I[I_COUNT])   
+        AUX_VALUE =  D_2 * BETA_K[I_COUNT] * MICRO * (Y_T0K[I_COUNT] - X_T0I[I_COUNT])    
+        NEW_VALUE += AUX_VALUE
+        X_T1I.append(NEW_VALUE) 
+    # Check boundes
+    X_T1I = META_CL.CHECK_INTERVAL_01(X_T1I, X_L, X_U) 
+    # Evaluation of the objective function and fitness
+    OF_T1I = OF_FUNCTION(X_T1I, NULL_DIC)
+    FIT_T1I = META_CL.FIT_VALUE(OF_T1I)
+    NEOF = 1
+    return X_T1I, OF_T1I, FIT_T1I, NEOF
+
+
+
+
+#   /$$$$$$  /$$$$$$$  /$$$$$$$$ /$$$$$$$$       /$$$$$$$$ /$$$$$$$$  /$$$$$$  /$$   /$$ /$$   /$$  /$$$$$$  /$$        /$$$$$$   /$$$$$$  /$$$$$$ /$$$$$$$$  /$$$$$$ 
+#  /$$__  $$| $$__  $$| $$_____/| $$_____/      |__  $$__/| $$_____/ /$$__  $$| $$  | $$| $$$ | $$ /$$__  $$| $$       /$$__  $$ /$$__  $$|_  $$_/| $$_____/ /$$__  $$
+# | $$  \__/| $$  \ $$| $$      | $$               | $$   | $$      | $$  \__/| $$  | $$| $$$$| $$| $$  \ $$| $$      | $$  \ $$| $$  \__/  | $$  | $$      | $$  \__/
+# | $$ /$$$$| $$$$$$$/| $$$$$   | $$$$$            | $$   | $$$$$   | $$      | $$$$$$$$| $$ $$ $$| $$  | $$| $$      | $$  | $$| $$ /$$$$  | $$  | $$$$$   |  $$$$$$ 
+# | $$|_  $$| $$____/ | $$__/   | $$__/            | $$   | $$__/   | $$      | $$__  $$| $$  $$$$| $$  | $$| $$      | $$  | $$| $$|_  $$  | $$  | $$__/    \____  $$
+# | $$  \ $$| $$      | $$      | $$               | $$   | $$      | $$    $$| $$  | $$| $$\  $$$| $$  | $$| $$      | $$  | $$| $$  \ $$  | $$  | $$       /$$  \ $$
+# |  $$$$$$/| $$      | $$$$$$$$| $$$$$$$$         | $$   | $$$$$$$$|  $$$$$$/| $$  | $$| $$ \  $$|  $$$$$$/| $$$$$$$$|  $$$$$$/|  $$$$$$/ /$$$$$$| $$$$$$$$|  $$$$$$/
 #  \______/ |__/      |________/|________/         |__/   |________/ \______/ |__/  |__/|__/  \__/ \______/ |________/ \______/  \______/ |______/|________/ \______/
```

### Comparing `META_TOOLBOX-2023.1/META_TOOLBOX/META_FUNCTIONS.py` & `META_TOOLBOX-2023.2/META_TOOLBOX/META_FUNCTIONS.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,261 +1,259 @@
-import numpy as np
-import matplotlib.pyplot as plt
-
-def SPHERE(X):
-    """
-    Sphere benchmark function d-dimension
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
-    """
-    
-    DIM = len(X)
-    SUM = 0
-    for I_COUNT in range(DIM):
-        X_I = X[I_COUNT]
-        SUM += X_I ** 2
-    OF = SUM
-    return OF
-
-def ROSENBROCK(X):
-    """
-    Rosenbrock benchmark function d-dimension.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
-    """
-    
-    DIM = len(X)
-    SUM = 0
-    for I_COUNT in range(DIM - 1):
-        X_I = X[I_COUNT]
-        X_NEXT = X[I_COUNT + 1]
-        NEW = 100 * (X_NEXT - X_I ** 2) ** 2 + (X_I - 1) ** 2
-        SUM += NEW
-    OF = SUM
-    return OF
-
-def RASTRIGIN(X):
-    """
-    Rastrigin benchmark function d-dimension.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
-    """
-    
-    DIM = len(X)
-    SUM = 0
-    for I_COUNT in range(DIM):
-        X_I = X[I_COUNT]
-        SUM += (X_I ** 2 - 10 * np.cos(2 * np.pi * X_I))
-    OF = 10 * DIM + SUM
-    return OF
-
-def ACKLEY(X):
-    """
-    Ackley benchmark function d-dimension.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
-    """
-    
-    DIM = len(X)
-    SUM1 = 0
-    SUM2 = 0
-    A = 20
-    B = 0.2
-    C = 2 * np.pi
-    for I_COUNT in range(DIM):
-        X_I = X[I_COUNT]
-        SUM1 += X_I ** 2
-        SUM2 += np.cos(C * X_I)
-    TERM_1 = -A * np.exp(-B * np.sqrt(SUM1 / DIM))
-    TERM_2 = -np.exp(SUM2 / DIM)
-    OF = TERM_1 + TERM_2 + A + np.exp(1)
-    return OF
-
-def GRIEWANK(X):
-    """
-    Griewank benchmark function d-dimension.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
-    """
-    
-    DIM = len(X)
-    SUM = 0
-    for I_COUNT in range(DIM):
-        X_I = X[I_COUNT]
-        SUM += (X_I ** 2) / 4000
-    PROD = np.cos(X_I / np.sqrt(X_I))
-    OF = SUM - PROD + 1
-    return OF
-
-def ZAKHAROV(X):
-    """
-    Zakharov benchmark function d-dimension.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
-    """
-    
-    DIM = len(X)
-    SUM_1 = 0
-    SUM_2 = 0
-    for I_COUNT in range(DIM):
-        X_I = X[I_COUNT]
-        SUM_1 += X_I ** 2
-        SUM_2 += (0.5 * I_COUNT * X_I)
-    OF = SUM_1 + SUM_2**2 + SUM_2**4
-    return OF
-
-def EASOM(X):
-    """
-    Easom benchmark function 2-dimension
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
-    """
-    
-    X_1 = X[0]
-    X_2 = X[1]
-    FACT_1 = - np.cos(X_1) * np.cos(X_2)
-    FACT_2 = np.exp(- (X_1 - np.pi) ** 2 - (X_2 - np.pi) ** 2)
-    OF = FACT_1 * FACT_2
-    return OF
-
-def MICHALEWICS(X):
-    """
-    Sphere benchmark function 2-dimension, 5-dimension and 10-dimension.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
-    """
-    
-    DIM = len(X)
-    SUM = 0
-    M = 10
-    for I_COUNT in range(DIM):
-        X_I = X[I_COUNT]
-        SUM += np.sin(X_I) * (np.sin((I_COUNT * X_I ** 2) / np.pi)**(2 * M))
-    OF = - SUM
-    return OF
-
-def RESIDUAL(S, O):
-    """
-    Residual value.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
-    """
-    return S - O
-
-def LOSS_FUNCTION_1(Y_EXP, Y_NUM):
-    """
-    Loss function d-dimension. Mean Square Error.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
-
-    https://search.r-project.org/CRAN/refmans/hydroGOF/html/mse.html
-    """
-    
-    ERROR = 0
-    for I in range(len(Y_EXP)):
-        RES = RESIDUAL(Y_NUM[I], Y_EXP[I])
-        ERROR += (RES) ** 2
-    OF = ERROR / len(Y_EXP)
-    
-    return OF
-
-def LOSS_FUNCTION_2(Y_EXP, Y_NUM):
-    """
-    Loss function d-dimension. Mean Absolute Error.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
-
-    https://search.r-project.org/CRAN/refmans/hydroGOF/html/mae.html
-    """
-    
-    ERROR = 0
-    for I in range(len(Y_EXP)):
-        RES = RESIDUAL(Y_NUM[I], Y_EXP[I])
-        ERROR += np.abs(RES)
-    OF = ERROR / len(Y_EXP)
-    
-    return OF
-
-def LOSS_FUNCTION_3(Y_EXP, Y_NUM):
-    """
-    Loss function d-dimension. Square Error.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
-    """
-    
-    ERROR = 0
-    for I in range(len(Y_EXP)):
-        RES = RESIDUAL(Y_NUM[I], Y_EXP[I])
-        ERROR += (RES) ** 2
-    OF = ERROR
-    
-    return OF
-
-def LOSS_FUNCTION_4(Y_EXP, Y_NUM, DELTA):
-    """
-    Loss function d-dimension. Smooth Mean Absolute Error or Hubber Loss.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
-    """
-
-    ERROR = 0
-    for I in range(len(Y_EXP)):
-        RES = RESIDUAL(Y_NUM[I], Y_EXP[I])
-        CRITERIA = np.abs(RES)
-        if CRITERIA <= DELTA:
-            ERROR += 0.5 * (RES) ** 2
-        else:
-            ERROR += DELTA * (np.abs(RES) - 0.5 * DELTA)
-    OF = ERROR
-    
-    return OF
-
-def LOSS_FUNCTION_5(Y_EXP, Y_NUM):
-    """
-    Loss function d-dimension. Root Mean Square Error.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
-    """
-    
-    ERROR = 0
-    for I in range(len(Y_EXP)):
-        RES = RESIDUAL(Y_NUM[I], Y_EXP[I])
-        ERROR += (RES) ** 2
-    OF = ERROR / len(Y_EXP)
-    OF = OF ** (0.5)
-    
-    return OF
-
-def LOSS_FUNCTION_6(Y_EXP, Y_NUM):
-    """
-    Loss function d-dimension. Mean Absolute Relative Error or Mean Magnitude Relative error.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
-
-    https://arxiv.org/ftp/arxiv/papers/1809/1809.03006.pdf
-    """
-    
-    ERROR = 0
-    for I in range(len(Y_EXP)):
-        RES = RESIDUAL(Y_NUM[I], Y_EXP[I])
-        ERROR += np.abs(RES) / np.abs(Y_EXP[I])
-    OF = ERROR / len(Y_EXP)
-    
-    return OF
-
-def LOSS_FUNCTION_7(Y_EXP, Y_NUM):
-    """
-    Loss function d-dimension. Normalized Root Mean Square Error.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
-
-    https://arxiv.org/ftp/arxiv/papers/1809/1809.03006.pdf
-    https://www.analyticsvidhya.com/blog/2021/10/evaluation-metric-for-regression-models/#:~:text=Relative%20Root%20Mean%20Square%20Error,to%20compare%20different%20measurement%20techniques.
-    """
-    
-    RMSE = LOSS_FUNCTION_5(Y_EXP, Y_NUM)
-    NVAL = np.std(Y_EXP)
-    OF = RMSE / NVAL
-    
-    return OF
-
+import numpy as np
+import matplotlib.pyplot as plt
+
+def SPHERE(X):
+    """
+    Sphere benchmark function d-dimension
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
+    """
+    
+    DIM = len(X)
+    SUM = 0
+    for I_COUNT in range(DIM):
+        X_I = X[I_COUNT]
+        SUM += X_I ** 2
+    OF = SUM
+    return OF
+
+def ROSENBROCK(X):
+    """
+    Rosenbrock benchmark function d-dimension.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
+    """
+    
+    DIM = len(X)
+    SUM = 0
+    for I_COUNT in range(DIM - 1):
+        X_I = X[I_COUNT]
+        X_NEXT = X[I_COUNT + 1]
+        NEW = 100 * (X_NEXT - X_I ** 2) ** 2 + (X_I - 1) ** 2
+        SUM += NEW
+    OF = SUM
+    return OF
+
+def RASTRIGIN(X):
+    """
+    Rastrigin benchmark function d-dimension.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
+    """
+    
+    DIM = len(X)
+    SUM = 0
+    for I_COUNT in range(DIM):
+        X_I = X[I_COUNT]
+        SUM += (X_I ** 2 - 10 * np.cos(2 * np.pi * X_I))
+    OF = 10 * DIM + SUM
+    return OF
+
+def ACKLEY(X):
+    """
+    Ackley benchmark function d-dimension.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
+    """
+    
+    DIM = len(X)
+    SUM1 = 0
+    SUM2 = 0
+    A = 20
+    B = 0.2
+    C = 2 * np.pi
+    for I_COUNT in range(DIM):
+        X_I = X[I_COUNT]
+        SUM1 += X_I ** 2
+        SUM2 += np.cos(C * X_I)
+    TERM_1 = -A * np.exp(-B * np.sqrt(SUM1 / DIM))
+    TERM_2 = -np.exp(SUM2 / DIM)
+    OF = TERM_1 + TERM_2 + A + np.exp(1)
+    return OF
+
+def GRIEWANK(X):
+    """
+    Griewank benchmark function d-dimension.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
+    """
+    
+    DIM = len(X)
+    SUM = 0
+    for I_COUNT in range(DIM):
+        X_I = X[I_COUNT]
+        SUM += (X_I ** 2) / 4000
+    PROD = np.cos(X_I / np.sqrt(X_I))
+    OF = SUM - PROD + 1
+    return OF
+
+def ZAKHAROV(X):
+    """
+    Zakharov benchmark function d-dimension.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
+    """
+    
+    DIM = len(X)
+    SUM_1 = 0
+    SUM_2 = 0
+    for I_COUNT in range(DIM):
+        X_I = X[I_COUNT]
+        SUM_1 += X_I ** 2
+        SUM_2 += (0.5 * I_COUNT * X_I)
+    OF = SUM_1 + SUM_2**2 + SUM_2**4
+    return OF
+
+def EASOM(X):
+    """
+    Easom benchmark function 2-dimension
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
+    """
+    
+    X_1 = X[0]
+    X_2 = X[1]
+    FACT_1 = - np.cos(X_1) * np.cos(X_2)
+    FACT_2 = np.exp(- (X_1 - np.pi) ** 2 - (X_2 - np.pi) ** 2)
+    OF = FACT_1 * FACT_2
+    return OF
+
+def MICHALEWICS(X):
+    """
+    Sphere benchmark function 2-dimension, 5-dimension and 10-dimension.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
+    """
+    
+    DIM = len(X)
+    SUM = 0
+    M = 10
+    for I_COUNT in range(DIM):
+        X_I = X[I_COUNT]
+        SUM += np.sin(X_I) * (np.sin((I_COUNT * X_I ** 2) / np.pi)**(2 * M))
+    OF = - SUM
+    return OF
+
+def RESIDUAL(S, O):
+    """
+    Residual value.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/008-BENCHMARKS.html
+    """
+    return S - O
+
+def LOSS_FUNCTION_1(Y_EXP, Y_NUM):
+    """
+    Loss function d-dimension. Mean Square Error.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/008-BENCHMARKS.html
+    """
+    
+    ERROR = 0
+    for I in range(len(Y_EXP)):
+        RES = RESIDUAL(Y_NUM[I], Y_EXP[I])
+        ERROR += (RES) ** 2
+    OF = ERROR / len(Y_EXP)
+    
+    return OF
+
+def LOSS_FUNCTION_2(Y_EXP, Y_NUM):
+    """
+    Loss function d-dimension. Mean Absolute Error.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
+
+    https://search.r-project.org/CRAN/refmans/hydroGOF/html/mae.html
+    """
+    
+    ERROR = 0
+    for I in range(len(Y_EXP)):
+        RES = RESIDUAL(Y_NUM[I], Y_EXP[I])
+        ERROR += np.abs(RES)
+    OF = ERROR / len(Y_EXP)
+    
+    return OF
+
+def LOSS_FUNCTION_3(Y_EXP, Y_NUM):
+    """
+    Loss function d-dimension. Square Error.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
+    """
+    
+    ERROR = 0
+    for I in range(len(Y_EXP)):
+        RES = RESIDUAL(Y_NUM[I], Y_EXP[I])
+        ERROR += (RES) ** 2
+    OF = ERROR
+    
+    return OF
+
+def LOSS_FUNCTION_4(Y_EXP, Y_NUM, DELTA):
+    """
+    Loss function d-dimension. Smooth Mean Absolute Error or Hubber Loss.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
+    """
+
+    ERROR = 0
+    for I in range(len(Y_EXP)):
+        RES = RESIDUAL(Y_NUM[I], Y_EXP[I])
+        CRITERIA = np.abs(RES)
+        if CRITERIA <= DELTA:
+            ERROR += 0.5 * (RES) ** 2
+        else:
+            ERROR += DELTA * (np.abs(RES) - 0.5 * DELTA)
+    OF = ERROR
+    
+    return OF
+
+def LOSS_FUNCTION_5(Y_EXP, Y_NUM):
+    """
+    Loss function d-dimension. Root Mean Square Error.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
+    """
+    
+    ERROR = 0
+    for I in range(len(Y_EXP)):
+        RES = RESIDUAL(Y_NUM[I], Y_EXP[I])
+        ERROR += (RES) ** 2
+    OF = ERROR / len(Y_EXP)
+    OF = OF ** (0.5)
+    
+    return OF
+
+def LOSS_FUNCTION_6(Y_EXP, Y_NUM):
+    """
+    Loss function d-dimension. Mean Absolute Relative Error or Mean Magnitude Relative error.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
+
+    https://arxiv.org/ftp/arxiv/papers/1809/1809.03006.pdf
+    """
+    
+    ERROR = 0
+    for I in range(len(Y_EXP)):
+        RES = RESIDUAL(Y_NUM[I], Y_EXP[I])
+        ERROR += np.abs(RES) / np.abs(Y_EXP[I])
+    OF = ERROR / len(Y_EXP)
+    
+    return OF
+
+def LOSS_FUNCTION_7(Y_EXP, Y_NUM):
+    """
+    Loss function d-dimension. Normalized Root Mean Square Error.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/BENCHMARKS.html
+
+    https://arxiv.org/ftp/arxiv/papers/1809/1809.03006.pdf
+    https://www.analyticsvidhya.com/blog/2021/10/evaluation-metric-for-regression-models/#:~:text=Relative%20Root%20Mean%20Square%20Error,to%20compare%20different%20measurement%20techniques.
+    """
+    
+    RMSE = LOSS_FUNCTION_5(Y_EXP, Y_NUM)
+    NVAL = np.std(Y_EXP)
+    OF = RMSE / NVAL
+    
+    return OF
+
 # Ler https://sci-hub.hkvisa.net/10.1016/j.rser.2015.11.058
```

### Comparing `META_TOOLBOX-2023.1/META_TOOLBOX/META_GRAPHICS_LIBRARY.py` & `META_TOOLBOX-2023.2/META_TOOLBOX/META_GRAPHICS_LIBRARY.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,419 +1,426 @@
-import matplotlib.pyplot as plt
-import numpy as np
-import seaborn as sns
-import META_TOOLBOX.META_FUNCTIONS as META_FN
-
-def CONVERT_SI_TO_INCHES(WIDTH, HEIGHT):
-    """ 
-    This function convert figure size meters to inches.
-    
-    Input:
-    WIDTH    |  Figure width in SI units       | Float
-    HEIGHT   |  Figure height in SI units      | Float
-    
-    Output:
-    WIDTH    |  Figure width in INCHES units   | Float
-    HEIGHT   |  Figure height in INCHES units  | Float
-    """
-    WIDTH = WIDTH / 0.0254
-    HEIGHT = HEIGHT / 0.0254
-    return WIDTH, HEIGHT
-
-def SAVE_GRAPHIC(NAME, EXT, DPI):
-    """ 
-    This function save graphics on a specific path extensions options.
-
-    Input: 
-    NAME  | Path + name figure               | String
-    EXT   | File extension                   | String
-		  |   '.svg'                         |
-          |   '.png'                         |
-          |   '.eps'                         |
-          |   '.pdf'                         |
-    DPI   | The resolution in dots per inch  | Integer
-    
-    Output:
-    N/A
-    """
-    plt.savefig(NAME + '.' + EXT, dpi = DPI, bbox_inches='tight', transparent=True)
-
-def META_PLOT_001(DATASET, PLOT_SETUP):
-	"""
-    OF + FIT chart - Line chart
-
-    Input:  
-    DATASET     | META Optimization toolbox results                        | Py dictionary
-	            |  Dictionary tags                                         |
-				|    'X'   = Values NEOF or Iterations                     | Py Numpy array[N_ITER + 1 x 1]
-	            |    'OF'  = Obj function value by iteration               | Py Numpy array[N_ITER + 1 x 1]
-                |    'FIT' = Fitness value by iteration                    | Py Numpy array[N_ITER + 1 x 1]
-    PLOT_SETUP  | Contains specifications of each model of chart           | Py Dictionary
-                |  Dictionary tags                                         |
-                |    'NAME'          == Filename output file               | String 
-                |    'WIDTH'         == Width figure                       | Float
-                |    'HEIGHT         == Height figure                      | Float
-                |    'EXTENSION'     == Extension output file              | String 
-                |    'DPI'           == Dots Per Inch - Image quality      | Integer   
-                |    'COLOR OF'      == OF line color                      | String
-				|    'MARKER OF'     == OF line marker                     | String
-                |    'COLOR FIT'     == FIT line color                     | String
-				|    'MARKER FIT'    == FIT line marker                    | String
-				|    'MARKER SIZE'   == Marker size                        | Float
-				|    'LINE WIDTH'    == Line width                         | Float
-				|    'LINE STYLE'    == Line style                         | String
-                |    'OF AXIS LABEL' == OF Y axis label name               | String
-                |    'X AXIS LABEL'  == X label name                       | String
-				|    'LABELS COLOR'  == Labels color                       | String
-				|    'LABELS SIZE'   == Labels size                        | Float
-                |    'X AXIS SIZE'   == X axis size                        | Float
-                |    'Y AXIS SIZE'   == Y axis size                        | Float
-                |    'AXISES COLOR'  == Axis color                         | String
-                |    'ON GRID?'      == Grid in chart                      | Boolean    
-				|    'Y LOG'         == Y axis logscale                    | Boolean     
-				|    'X LOG'         == X axis logscale                    | Boolean 
-    
-    Output:
-    The image is saved in the current directory 
-	"""
-	NAME = PLOT_SETUP['NAME']
-	W = PLOT_SETUP['WIDTH']
-	H = PLOT_SETUP['HEIGHT']
-	EXT = PLOT_SETUP['EXTENSION']
-	DPI = PLOT_SETUP['DPI']
-	COLOR_OF = PLOT_SETUP['COLOR OF']
-	MARKER_OF = PLOT_SETUP['MARKER OF']
-	COLOR_FIT = PLOT_SETUP['COLOR FIT']
-	MARKER_FIT = PLOT_SETUP['MARKER FIT']
-	MARKER_SIZE = PLOT_SETUP['MARKER SIZE']
-	LINE_WIDTH = PLOT_SETUP['LINE WIDTH']
-	LINE_STYLE = PLOT_SETUP['LINE STYLE']
-	Y_OF_AXIS_LABEL = PLOT_SETUP['OF AXIS LABEL']
-	X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']
-	LABELS_SIZE = PLOT_SETUP['LABELS SIZE']     
-	LABELS_COLOR = PLOT_SETUP['LABELS COLOR']
-	X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
-	Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']
-	AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
-	YLOGSCALE = PLOT_SETUP['Y LOG']
-	XLOGSCALE = PLOT_SETUP['X LOG']
-	GRID = PLOT_SETUP['ON GRID?']
-	X = DATASET['X']
-	Y_0 = DATASET['OF']
-	Y_1 = DATASET['FIT']
-	
-	# Convert units of size figure
-	W, H = CONVERT_SI_TO_INCHES(W, H)
-	
-	# Plot
-	FIG, AX = plt.subplots(2, 1, figsize = (W, H), sharex = True)
-	AX[0].plot(X, Y_0, marker = MARKER_OF, color = COLOR_OF, linestyle = LINE_STYLE, linewidth = LINE_WIDTH, markersize = MARKER_SIZE)
-	AX[1].plot(X, Y_1, marker = MARKER_FIT, color = COLOR_FIT, linestyle = LINE_STYLE, linewidth = LINE_WIDTH, markersize = MARKER_SIZE)
-	if YLOGSCALE:
-		AX[0].semilogy()
-		AX[1].semilogy()
-	if XLOGSCALE:
-		AX[0].semilogx()
-		AX[1].semilogx()
-	font = {'fontname': 'Arial',
-			'color':  LABELS_COLOR,
-			'weight': 'normal',
-			'size': LABELS_SIZE}
-	AX[0].set_ylabel(Y_OF_AXIS_LABEL, fontdict = font)
-	AX[1].set_xlabel(X_AXIS_LABEL, fontdict = font)
-	AX[1].set_ylabel('$Fitness$', fontdict = font)          
-	AX[0].tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
-	AX[0].tick_params(axis = 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
-	AX[1].tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
-	AX[1].tick_params(axis = 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
-	if GRID == True:
-		AX[0].grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
-		AX[1].grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
-	SAVE_GRAPHIC(NAME, EXT, DPI)
-
-def META_PLOT_002(DATASET, PLOT_SETUP):
-	"""
-    OF or FIT chart - Line chart
-
-    Input:  
-    DATASET     | META Optimization toolbox results                        | Py dictionary
-	            |  Dictionary tags                                         |
-				|    'X'   = Values NEOF or Iterations                     | Py Numpy array[N_ITER + 1 x 1]
-	            |    'Y'  = Obj, Fit, Worst or average value by iteration  | Py Numpy array[N_ITER + 1 x 1]
-    PLOT_SETUP  | Contains specifications of each model of chart           | Py Dictionary
-                |  Dictionary tags                                         |
-                |    'NAME'          == Filename output file               | String 
-                |    'WIDTH'         == Width figure                       | Float
-                |    'HEIGHT         == Height figure                      | Float
-                |    'EXTENSION'     == Extension output file              | String 
-                |    'DPI'           == Dots Per Inch - Image quality      | Integer   
-                |    'COLOR'         == Line color                         | String
-				|    'MARKER'        == Line marker                        | String
-				|    'MARKER SIZE'   == Marker size                        | Float
-				|    'LINE WIDTH'    == Line width                         | Float
-				|    'LINE STYLE'    == Line style                         | String
-                |    'Y AXIS LABEL'  == Y axis label name                  | String
-                |    'X AXIS LABEL'  == X axis label name                  | String
-				|    'LABELS COLOR'  == Labels color                       | String
-				|    'LABELS SIZE'   == Labels size                        | Float
-                |    'X AXIS SIZE'   == X axis size                        | Float
-                |    'Y AXIS SIZE'   == Y axis size                        | Float
-                |    'AXISES COLOR'  == Axis color                         | String
-                |    'ON GRID?'      == Grid in chart                      | Boolean  
-				|    'Y LOG'         == Y axis logscale                    | Boolean     
-				|    'X LOG'         == X axis logscale                    | Boolean 
-    
-    Output:
-    The image is saved in the current directory 
-	"""
-	NAME = PLOT_SETUP['NAME']
-	W = PLOT_SETUP['WIDTH']
-	H = PLOT_SETUP['HEIGHT']
-	EXT = PLOT_SETUP['EXTENSION']
-	DPI = PLOT_SETUP['DPI']
-	COLOR = PLOT_SETUP['COLOR']
-	MARKER = PLOT_SETUP['MARKER']
-	MARKER_SIZE = PLOT_SETUP['MARKER SIZE']
-	LINE_WIDTH = PLOT_SETUP['LINE WIDTH']
-	LINE_STYLE = PLOT_SETUP['LINE STYLE']
-	Y_AXIS_LABEL = PLOT_SETUP['Y AXIS LABEL']
-	X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']
-	LABELS_SIZE = PLOT_SETUP['LABELS SIZE']     
-	LABELS_COLOR = PLOT_SETUP['LABELS COLOR']
-	X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
-	Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']
-	AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
-	GRID = PLOT_SETUP['ON GRID?']
-	YLOGSCALE = PLOT_SETUP['Y LOG']
-	XLOGSCALE = PLOT_SETUP['X LOG']
-	X = DATASET['X']
-	Y = DATASET['Y']
-	
-	# Convert units of size figure
-	W, H = CONVERT_SI_TO_INCHES(W, H)
-	
-	# Plot
-	FIG, AX = plt.subplots(1, 1, figsize = (W, H), sharex = True)
-	AX.plot(X, Y, marker = MARKER, color = COLOR, linestyle = LINE_STYLE, linewidth = LINE_WIDTH, markersize = MARKER_SIZE)
-	if YLOGSCALE:
-		AX.semilogy()
-	if XLOGSCALE:
-		AX.semilogx()
-	font = {'fontname': 'Arial',
-			'color':  LABELS_COLOR,
-			'weight': 'normal',
-			'size': LABELS_SIZE}
-	AX.set_ylabel(Y_AXIS_LABEL, fontdict = font)
-	AX.set_xlabel(X_AXIS_LABEL, fontdict = font)   
-	AX.tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
-	AX.tick_params(axis = 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
-	if GRID == True:
-		AX.grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
-	SAVE_GRAPHIC(NAME, EXT, DPI)
-
-def META_PLOT_003(DATASET, PLOT_SETUP):
-	"""
-    OF or FIT - Line chart
-
-    Input:  
-    DATASET     | META Optimization toolbox results                        | Py dictionary
-	            |  Dictionary tags                                         |
-				|    'X'     = Values NEOF or Iterations                   | Py Numpy array[N_ITER + 1 x 1]
-	            |    'BEST'  = Best value by iteration                     | Py Numpy array[N_ITER + 1 x 1]
-	            |    'WORST'  = Best value by iteration                    | Py Numpy array[N_ITER + 1 x 1]
-	            |    'AVERAGE'  = Best value by iteration                  | Py Numpy array[N_ITER + 1 x 1]
-    PLOT_SETUP  | Contains specifications of each model of chart           | Py Dictionary
-                |  Dictionary tags                                         |
-                |    'NAME'          == Filename output file               | String 
-                |    'WIDTH'         == Width figure                       | Float
-                |    'HEIGHT         == Height figure                      | Float
-                |    'EXTENSION'     == Extension output file              | String 
-                |    'DPI'           == Dots Per Inch - Image quality      | Integer   
-                |    'COLOR BEST'    == Line color - Best results          | String
-            	|    'COLOR WORST'   == Line color - Worst results         | String	
-                |    'COLOR AVERAGE' == Line color - Average results       | String
-				|    'MARKER'        == Line marker                        | String
-				|    'MARKER SIZE'   == Marker size                        | Float
-				|    'LINE WIDTH'    == Line width                         | Float
-				|    'LINE STYLE'    == Line style                         | String
-                |    'Y AXIS LABEL'  == Y axis label name                  | String
-                |    'X AXIS LABEL'  == X axis label name                  | String
-				|    'LABELS COLOR'  == Labels color                       | String
-				|    'LABELS SIZE'   == Labels size                        | Float
-                |    'X AXIS SIZE'   == X axis size                        | Float
-                |    'Y AXIS SIZE'   == Y axis size                        | Float
-                |    'AXISES COLOR'  == Axis color                         | String
-                |    'GRID'          == Grid in chart                      | Boolean  
-				|    'Y LOG'         == Y axis logscale                    | Boolean 
-				|    'X LOG'         == X axis logscale                    | Boolean 
-				|    LOC LEGEND      == Legend location                    | String
-				|    SIZE LEGEND     == Legend size                        | Float
-    
-    Output:
-    The image is saved in the current directory 
-	"""
-	NAME = PLOT_SETUP['NAME']
-	W = PLOT_SETUP['WIDTH']
-	H = PLOT_SETUP['HEIGHT']
-	EXT = PLOT_SETUP['EXTENSION']
-	DPI = PLOT_SETUP['DPI']
-	COLOR_1 = PLOT_SETUP['COLOR BEST']
-	COLOR_2 = PLOT_SETUP['COLOR WORST']
-	COLOR_3 = PLOT_SETUP['COLOR AVERAGE']
-	MARKER = PLOT_SETUP['MARKER']
-	MARKER_SIZE = PLOT_SETUP['MARKER SIZE']
-	LINE_WIDTH = PLOT_SETUP['LINE WIDTH']
-	LINE_STYLE = PLOT_SETUP['LINE STYLE']
-	Y_AXIS_LABEL = PLOT_SETUP['Y AXIS LABEL']
-	X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']
-	LABELS_SIZE = PLOT_SETUP['LABELS SIZE']     
-	LABELS_COLOR = PLOT_SETUP['LABELS COLOR']
-	X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
-	Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']
-	AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
-	GRID = PLOT_SETUP['ON GRID?']
-	YLOGSCALE = PLOT_SETUP['Y LOG']
-	XLOGSCALE = PLOT_SETUP['X LOG']
-	LOC = PLOT_SETUP['LOC LEGEND']
-	SIZE_LEGEND = PLOT_SETUP['SIZE LEGEND']
-	X = DATASET['X']
-	Y_1 = DATASET['BEST']
-	Y_2 = DATASET['WORST']
-	Y_3 = DATASET['AVERAGE']
-	
-	# Convert units of size figure
-	W, H = CONVERT_SI_TO_INCHES(W, H)
-	
-	# Plot
-	FIG, AX= plt.subplots(1, 1, figsize = (W, H), sharex = True)
-	AX.plot(X, Y_1, marker = MARKER, color = COLOR_1, linestyle = LINE_STYLE, linewidth = LINE_WIDTH, markersize = MARKER_SIZE, label='Best')
-	AX.plot(X, Y_2, marker = MARKER, color = COLOR_2, linestyle = LINE_STYLE, linewidth = LINE_WIDTH, markersize = MARKER_SIZE, label='Worst')
-	AX.plot(X, Y_3, marker = MARKER, color = COLOR_3, linestyle = LINE_STYLE, linewidth = LINE_WIDTH, markersize = MARKER_SIZE, label='Average')
-	if YLOGSCALE:
-		AX.semilogy()
-	if XLOGSCALE:
-		AX.semilogx()
-	font = {'fontname': 'Arial',
-			'color':  LABELS_COLOR,
-			'weight': 'normal',
-			'size': LABELS_SIZE}
-	AX.set_ylabel(Y_AXIS_LABEL, fontdict = font)
-	AX.set_xlabel(X_AXIS_LABEL, fontdict = font)   
-	AX.tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
-	AX.tick_params(axis = 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
-	if GRID == True:
-		AX.grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
-	plt.legend(loc = LOC, prop = {'size': SIZE_LEGEND})
-	SAVE_GRAPHIC(NAME, EXT, DPI)
-
-def META_PLOT_004(DATASET, PLOT_SETUP):
-    """
-    OF or FIT - Boxplot and histogram
-
-	Input:
-    DATASET     | Results from a RASD Toolboox                              | Py dataframe or Py Numpy array[N_POP x 1]
-                |    Dictionary tags                                        |
-                |    'DATA'          == Complete data                       | Py Numpy array[N_POP x 1]
-                |    'COLUMN'        == Dataframe column                    | String
-    PLOT_SETUP  | Contains specifications of each model of chart            | Py dictionary
-                |    Dictionary tags                                        |
-                |    'NAME'          == Filename output file                | String 
-                |    'WIDTH'         == Width figure                        | Float
-                |    'HEIGHT         == Height figure                       | Float
-                |    'X AXIS SIZE'   == X axis size                         | Float
-                |    'Y AXIS SIZE'   == Y axis size                         | Float
-                |    'AXISES COLOR'  == Axis color                          | String
-                |    'X AXIS LABEL'  == X label name                        | String
-                |    'LABELS SIZE'   == Labels size                         | Float
-                |    'LABELS COLOR'  == Labels color                        | String
-                |    'CHART COLOR'   == Boxplot and histogram color         | String
-                |    'BINS'          == Range representing the width of     | Float
-                |                       a single bar                        | 
-                |    'KDE'           == Smooth of the random distribution   | Boolean      
-                |    'DPI'           == Dots Per Inch - Image quality       | Integer   
-                |    'EXTENSION'     == Extension output file               | String ('.svg, '.png', '.eps' or '.pdf')
-
-    Output:
-    The image is saved in the current directory 
-    """
-    
-	# Checking which is the best process 
-    MINVALUES = []
-    N_REP = DATASET['NUMBER OF REPETITIONS']
-    N_ITER = DATASET['NUMBER OF ITERATIONS']
-    TYPE = DATASET['OF OR FIT']
-    BEST_REP = DATASET['BEST']
-    for ID in range(N_REP):
-        if TYPE == 'OF':
-            X = BEST_REP[ID]['OF'][N_ITER]
-        else:
-            X = BEST_REP[ID]['FIT'][N_ITER]
-        MINVALUES.append(X)
-    NAME = PLOT_SETUP['NAME']
-    W = PLOT_SETUP['WIDTH']
-    H = PLOT_SETUP['HEIGHT']
-    EXT = PLOT_SETUP['EXTENSION']
-    DPI = PLOT_SETUP['DPI']
-    X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']
-    X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
-    Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']
-    AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
-    LABELS_SIZE = PLOT_SETUP['LABELS SIZE']     
-    LABELS_COLOR = PLOT_SETUP['LABELS COLOR']
-    CHART_COLOR = PLOT_SETUP['COLOR']
-    BINS = PLOT_SETUP['BINS']
-    KDE = PLOT_SETUP['KDE']
-
-    sns.set(style = 'ticks')
-
-    # Convert units of size figure
-    [W, H] = CONVERT_SI_TO_INCHES(W, H)
-    
-	# Plot
-    FIG, (AX_BOX, AX_HIST) = plt.subplots(2, figsize = (W, H), sharex = True, gridspec_kw = {'height_ratios': (.15, .85)})
-    sns.boxplot(MINVALUES, ax = AX_BOX, color = CHART_COLOR)
-    sns.histplot(MINVALUES, ax = AX_HIST, kde = KDE, color = CHART_COLOR, bins = BINS)
-    AX_BOX.set(yticks = [])
-    AX_BOX.set(xlabel='')
-    font = {'fontname': 'Arial',
-            'color':  LABELS_COLOR,
-            'weight': 'normal',
-            'size': LABELS_SIZE}
-    AX_HIST.set_xlabel(X_AXIS_LABEL, fontdict = font)
-    AX_HIST.set_ylabel('$Frequency$', fontdict = font)
-    AX_HIST.tick_params(axis= 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
-    AX_HIST.tick_params(axis= 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
-    sns.despine(ax = AX_HIST)
-    sns.despine(ax = AX_BOX, left = True)
-    SAVE_GRAPHIC(NAME, EXT, DPI)
-
-def META_PLOT_005(X,FUNCTION,X_L, X_U):
-    N = 100
-    X_AUX = np.linspace(X_L, X_U, N)
-    Y_AUX = np.linspace(X_L, X_U, N)
-    A, B = np.meshgrid(X_AUX, Y_AUX)
-    Z = np.zeros((N,N))
-    for I in range(N):
-        for J in range(N):
-            X = [A[I, J], B[I, J]]
-            if FUNCTION == "ACKLEY":
-                Z[I, J] = META_FN.ACKLEY(X)
-            if FUNCTION == "SPHERE":
-                Z[I, J] = META_FN.SPHERE(X)
-            if FUNCTION == "ROSENBROCK":
-                Z[I, J] = META_FN.ROSENBROCK(X)
-            if FUNCTION == "RASTRIGIN":
-                Z[I, J] = META_FN.RASTRIGIN(X)
-            if FUNCTION == "GRIEWANK":
-                Z[I, J] = META_FN.GRIEWANK(X)
-            if FUNCTION == "ZAKHAROV":
-                Z[I, J] = META_FN.ZAKHAROV(X)
-            if FUNCTION == "EASOM":
-                Z[I, J] = META_FN.EASOM(X)
-            if FUNCTION == "MICHALEWICS":
-                Z[I, J] = META_FN.MICHALEWICS(X)
-    fig = plt.figure()
-    ax = plt.axes(projection = '3d')
-    ax.contour3D(A, B, Z, 100, cmap = 'jet')
-    ax.set_xlabel('x')
-    ax.set_ylabel('y')
-    ax.set_zlabel('z');
+import matplotlib.pyplot as plt
+import numpy as np
+import seaborn as sns
+import META_TOOLBOX.META_FUNCTIONS as META_FN
+
+def CONVERT_SI_TO_INCHES(WIDTH, HEIGHT):
+    """ 
+    This function convert figure size meters to inches.
+    
+    Input:
+    WIDTH    |  Figure width in SI units       | Float
+    HEIGHT   |  Figure height in SI units      | Float
+    
+    Output:
+    WIDTH    |  Figure width in INCHES units   | Float
+    HEIGHT   |  Figure height in INCHES units  | Float
+    """
+    WIDTH = WIDTH / 0.0254
+    HEIGHT = HEIGHT / 0.0254
+    return WIDTH, HEIGHT
+
+def SAVE_GRAPHIC(NAME, EXT, DPI):
+    """ 
+    This function save graphics on a specific path extensions options.
+
+    Input: 
+    NAME  | Path + name figure               | String
+    EXT   | File extension                   | String
+		  |   'svg'                         |
+          |   'png'                         |
+          |   'eps'                         |
+          |   'pdf'                         |
+    DPI   | The resolution in dots per inch  | Integer
+    
+    Output:
+    N/A
+    """
+    plt.savefig(NAME + '.' + EXT, dpi = DPI, bbox_inches='tight', transparent=True)
+
+def META_PLOT_001(DATASET, PLOT_SETUP):
+	"""
+    OF + FIT chart - Line chart
+
+    Input:  
+    DATASET     | META Optimization toolbox results                        | Py dictionary
+	            |  Dictionary tags                                         |
+				|    'X'   = Values NEOF or Iterations                     | Py Numpy array[N_ITER + 1 x 1]
+	            |    'OF'  = Obj function value by iteration               | Py Numpy array[N_ITER + 1 x 1]
+                |    'FIT' = Fitness value by iteration                    | Py Numpy array[N_ITER + 1 x 1]
+    PLOT_SETUP  | Contains specifications of each model of chart           | Py Dictionary
+                |  Dictionary tags                                         |
+                |    'NAME'          == Filename output file               | String 
+                |    'WIDTH'         == Width figure                       | Float
+                |    'HEIGHT         == Height figure                      | Float
+                |    'EXTENSION'     == Extension output file              | String 
+                |    'DPI'           == Dots Per Inch - Image quality      | Integer   
+                |    'COLOR OF'      == OF line color                      | String
+				|    'MARKER OF'     == OF line marker                     | String
+                |    'COLOR FIT'     == FIT line color                     | String
+				|    'MARKER FIT'    == FIT line marker                    | String
+				|    'MARKER SIZE'   == Marker size                        | Float
+				|    'LINE WIDTH'    == Line width                         | Float
+				|    'LINE STYLE'    == Line style                         | String
+                |    'OF AXIS LABEL' == OF Y axis label name               | String
+                |    'X AXIS LABEL'  == X label name                       | String
+				|    'LABELS COLOR'  == Labels color                       | String
+				|    'LABELS SIZE'   == Labels size                        | Float
+                |    'X AXIS SIZE'   == X axis size                        | Float
+                |    'Y AXIS SIZE'   == Y axis size                        | Float
+                |    'AXISES COLOR'  == Axis color                         | String
+                |    'ON GRID?'      == Grid in chart                      | Boolean    
+				|    'Y LOG'         == Y axis logscale                    | Boolean     
+				|    'X LOG'         == X axis logscale                    | Boolean 
+    
+    Output:
+    The image is saved in the current directory 
+	"""
+	NAME = PLOT_SETUP['NAME']
+	W = PLOT_SETUP['WIDTH']
+	H = PLOT_SETUP['HEIGHT']
+	EXT = PLOT_SETUP['EXTENSION']
+	DPI = PLOT_SETUP['DPI']
+	COLOR_OF = PLOT_SETUP['COLOR OF']
+	MARKER_OF = PLOT_SETUP['MARKER OF']
+	COLOR_FIT = PLOT_SETUP['COLOR FIT']
+	MARKER_FIT = PLOT_SETUP['MARKER FIT']
+	MARKER_SIZE = PLOT_SETUP['MARKER SIZE']
+	LINE_WIDTH = PLOT_SETUP['LINE WIDTH']
+	LINE_STYLE = PLOT_SETUP['LINE STYLE']
+	Y_OF_AXIS_LABEL = PLOT_SETUP['OF AXIS LABEL']
+	X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']
+	LABELS_SIZE = PLOT_SETUP['LABELS SIZE']     
+	LABELS_COLOR = PLOT_SETUP['LABELS COLOR']
+	X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
+	Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']
+	AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
+	YLOGSCALE = PLOT_SETUP['Y LOG']
+	XLOGSCALE = PLOT_SETUP['X LOG']
+	GRID = PLOT_SETUP['ON GRID?']
+	X = DATASET['X']
+	Y_0 = DATASET['OF']
+	Y_1 = DATASET['FIT']
+	
+	# Convert units of size figure
+	W, H = CONVERT_SI_TO_INCHES(W, H)
+	
+	# Plot
+	FIG, AX = plt.subplots(2, 1, figsize = (W, H), sharex = True)
+	AX[0].plot(X, Y_0, marker = MARKER_OF, color = COLOR_OF, linestyle = LINE_STYLE, linewidth = LINE_WIDTH, markersize = MARKER_SIZE)
+	AX[1].plot(X, Y_1, marker = MARKER_FIT, color = COLOR_FIT, linestyle = LINE_STYLE, linewidth = LINE_WIDTH, markersize = MARKER_SIZE)
+	if YLOGSCALE:
+		AX[0].semilogy()
+		AX[1].semilogy()
+	if XLOGSCALE:
+		AX[0].semilogx()
+		AX[1].semilogx()
+	font = {'fontname': 'Arial',
+			'color':  LABELS_COLOR,
+			'weight': 'normal',
+			'size': LABELS_SIZE}
+	AX[0].set_ylabel(Y_OF_AXIS_LABEL, fontdict = font)
+	AX[1].set_xlabel(X_AXIS_LABEL, fontdict = font)
+	AX[1].set_ylabel('$Fitness$', fontdict = font)          
+	AX[0].tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
+	AX[0].tick_params(axis = 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
+	AX[1].tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
+	AX[1].tick_params(axis = 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
+	if GRID == True:
+		AX[0].grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
+		AX[1].grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
+	SAVE_GRAPHIC(NAME, EXT, DPI)
+
+def META_PLOT_002(DATASET, PLOT_SETUP):
+	"""
+    OF or FIT chart - Line chart
+
+    Input:  
+    DATASET     | META Optimization toolbox results                        | Py dictionary
+	            |  Dictionary tags                                         |
+				|    'X'   = Values NEOF or Iterations                     | Py Numpy array[N_ITER + 1 x 1]
+	            |    'Y'  = Obj, Fit, Worst or average value by iteration  | Py Numpy array[N_ITER + 1 x 1]
+    PLOT_SETUP  | Contains specifications of each model of chart           | Py Dictionary
+                |  Dictionary tags                                         |
+                |    'NAME'          == Filename output file               | String 
+                |    'WIDTH'         == Width figure                       | Float
+                |    'HEIGHT         == Height figure                      | Float
+                |    'EXTENSION'     == Extension output file              | String 
+                |    'DPI'           == Dots Per Inch - Image quality      | Integer   
+                |    'COLOR'         == Line color                         | String
+				|    'MARKER'        == Line marker                        | String
+				|    'MARKER SIZE'   == Marker size                        | Float
+				|    'LINE WIDTH'    == Line width                         | Float
+				|    'LINE STYLE'    == Line style                         | String
+                |    'Y AXIS LABEL'  == Y axis label name                  | String
+                |    'X AXIS LABEL'  == X axis label name                  | String
+				|    'LABELS COLOR'  == Labels color                       | String
+				|    'LABELS SIZE'   == Labels size                        | Float
+                |    'X AXIS SIZE'   == X axis size                        | Float
+                |    'Y AXIS SIZE'   == Y axis size                        | Float
+                |    'AXISES COLOR'  == Axis color                         | String
+                |    'ON GRID?'      == Grid in chart                      | Boolean  
+				|    'Y LOG'         == Y axis logscale                    | Boolean     
+				|    'X LOG'         == X axis logscale                    | Boolean 
+    
+    Output:
+    The image is saved in the current directory 
+	"""
+	NAME = PLOT_SETUP['NAME']
+	W = PLOT_SETUP['WIDTH']
+	H = PLOT_SETUP['HEIGHT']
+	EXT = PLOT_SETUP['EXTENSION']
+	DPI = PLOT_SETUP['DPI']
+	COLOR = PLOT_SETUP['COLOR']
+	MARKER = PLOT_SETUP['MARKER']
+	MARKER_SIZE = PLOT_SETUP['MARKER SIZE']
+	LINE_WIDTH = PLOT_SETUP['LINE WIDTH']
+	LINE_STYLE = PLOT_SETUP['LINE STYLE']
+	Y_AXIS_LABEL = PLOT_SETUP['Y AXIS LABEL']
+	X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']
+	LABELS_SIZE = PLOT_SETUP['LABELS SIZE']     
+	LABELS_COLOR = PLOT_SETUP['LABELS COLOR']
+	X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
+	Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']
+	AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
+	GRID = PLOT_SETUP['ON GRID?']
+	YLOGSCALE = PLOT_SETUP['Y LOG']
+	XLOGSCALE = PLOT_SETUP['X LOG']
+	X = DATASET['X']
+	Y = DATASET['Y']
+	
+	# Convert units of size figure
+	W, H = CONVERT_SI_TO_INCHES(W, H)
+	
+	# Plot
+	FIG, AX = plt.subplots(1, 1, figsize = (W, H), sharex = True)
+	AX.plot(X, Y, marker = MARKER, color = COLOR, linestyle = LINE_STYLE, linewidth = LINE_WIDTH, markersize = MARKER_SIZE)
+	if YLOGSCALE:
+		AX.semilogy()
+	if XLOGSCALE:
+		AX.semilogx()
+	font = {'fontname': 'Arial',
+			'color':  LABELS_COLOR,
+			'weight': 'normal',
+			'size': LABELS_SIZE}
+	AX.set_ylabel(Y_AXIS_LABEL, fontdict = font)
+	AX.set_xlabel(X_AXIS_LABEL, fontdict = font)   
+	AX.tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
+	AX.tick_params(axis = 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
+	if GRID == True:
+		AX.grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
+	SAVE_GRAPHIC(NAME, EXT, DPI)
+
+def META_PLOT_003(DATASET, PLOT_SETUP):
+	"""
+    OF or FIT - Line chart
+
+    Input:  
+    DATASET     | META Optimization toolbox results                        | Py dictionary
+	            |  Dictionary tags                                         |
+				|    'X'     = Values NEOF or Iterations                   | Py Numpy array[N_ITER + 1 x 1]
+	            |    'BEST'  = Best value by iteration                     | Py Numpy array[N_ITER + 1 x 1]
+	            |    'WORST'  = Best value by iteration                    | Py Numpy array[N_ITER + 1 x 1]
+	            |    'AVERAGE'  = Best value by iteration                  | Py Numpy array[N_ITER + 1 x 1]
+    PLOT_SETUP  | Contains specifications of each model of chart           | Py Dictionary
+                |  Dictionary tags                                         |
+                |    'NAME'          == Filename output file               | String 
+                |    'WIDTH'         == Width figure                       | Float
+                |    'HEIGHT         == Height figure                      | Float
+                |    'EXTENSION'     == Extension output file              | String 
+                |    'DPI'           == Dots Per Inch - Image quality      | Integer   
+                |    'COLOR BEST'    == Line color - Best results          | String
+            	|    'COLOR WORST'   == Line color - Worst results         | String	
+                |    'COLOR AVERAGE' == Line color - Average results       | String
+				|    'MARKER'        == Line marker                        | String
+				|    'MARKER SIZE'   == Marker size                        | Float
+				|    'LINE WIDTH'    == Line width                         | Float
+				|    'LINE STYLE'    == Line style                         | String
+                |    'Y AXIS LABEL'  == Y axis label name                  | String
+                |    'X AXIS LABEL'  == X axis label name                  | String
+				|    'LABELS COLOR'  == Labels color                       | String
+				|    'LABELS SIZE'   == Labels size                        | Float
+                |    'X AXIS SIZE'   == X axis size                        | Float
+                |    'Y AXIS SIZE'   == Y axis size                        | Float
+                |    'AXISES COLOR'  == Axis color                         | String
+                |    'GRID'          == Grid in chart                      | Boolean  
+				|    'Y LOG'         == Y axis logscale                    | Boolean 
+				|    'X LOG'         == X axis logscale                    | Boolean 
+				|    LOC LEGEND      == Legend location                    | String
+				|    SIZE LEGEND     == Legend size                        | Float
+    
+    Output:
+    The image is saved in the current directory 
+	"""
+	NAME = PLOT_SETUP['NAME']
+	W = PLOT_SETUP['WIDTH']
+	H = PLOT_SETUP['HEIGHT']
+	EXT = PLOT_SETUP['EXTENSION']
+	DPI = PLOT_SETUP['DPI']
+	COLOR_1 = PLOT_SETUP['COLOR BEST']
+	COLOR_2 = PLOT_SETUP['COLOR WORST']
+	COLOR_3 = PLOT_SETUP['COLOR AVERAGE']
+	MARKER = PLOT_SETUP['MARKER']
+	MARKER_SIZE = PLOT_SETUP['MARKER SIZE']
+	LINE_WIDTH = PLOT_SETUP['LINE WIDTH']
+	LINE_STYLE = PLOT_SETUP['LINE STYLE']
+	Y_AXIS_LABEL = PLOT_SETUP['Y AXIS LABEL']
+	X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']
+	LABELS_SIZE = PLOT_SETUP['LABELS SIZE']     
+	LABELS_COLOR = PLOT_SETUP['LABELS COLOR']
+	X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
+	Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']
+	AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
+	GRID = PLOT_SETUP['ON GRID?']
+	YLOGSCALE = PLOT_SETUP['Y LOG']
+	XLOGSCALE = PLOT_SETUP['X LOG']
+	LOC = PLOT_SETUP['LOC LEGEND']
+	SIZE_LEGEND = PLOT_SETUP['SIZE LEGEND']
+	X = DATASET['X']
+	Y_1 = DATASET['BEST']
+	Y_2 = DATASET['WORST']
+	Y_3 = DATASET['AVERAGE']
+	
+	# Convert units of size figure
+	W, H = CONVERT_SI_TO_INCHES(W, H)
+	
+	# Plot
+	FIG, AX= plt.subplots(1, 1, figsize = (W, H), sharex = True)
+	AX.plot(X, Y_1, marker = MARKER, color = COLOR_1, linestyle = LINE_STYLE, linewidth = LINE_WIDTH, markersize = MARKER_SIZE, label='Best')
+	AX.plot(X, Y_2, marker = MARKER, color = COLOR_2, linestyle = LINE_STYLE, linewidth = LINE_WIDTH, markersize = MARKER_SIZE, label='Worst')
+	AX.plot(X, Y_3, marker = MARKER, color = COLOR_3, linestyle = LINE_STYLE, linewidth = LINE_WIDTH, markersize = MARKER_SIZE, label='Average')
+	if YLOGSCALE:
+		AX.semilogy()
+	if XLOGSCALE:
+		AX.semilogx()
+	font = {'fontname': 'Arial',
+			'color':  LABELS_COLOR,
+			'weight': 'normal',
+			'size': LABELS_SIZE}
+	AX.set_ylabel(Y_AXIS_LABEL, fontdict = font)
+	AX.set_xlabel(X_AXIS_LABEL, fontdict = font)   
+	AX.tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
+	AX.tick_params(axis = 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
+	if GRID == True:
+		AX.grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
+	plt.legend(loc = LOC, prop = {'size': SIZE_LEGEND})
+	SAVE_GRAPHIC(NAME, EXT, DPI)
+
+def META_PLOT_004(DATASET, PLOT_SETUP):
+    """
+    OF or FIT - Boxplot and histogram
+
+	Input:
+    DATASET     | Results from a RASD Toolboox                              | Py dataframe or Py Numpy array[N_POP x 1]
+                |    Dictionary tags                                        |
+                |    'DATA'          == Complete data                       | Py Numpy array[N_POP x 1]
+                |    'COLUMN'        == Dataframe column                    | String
+    PLOT_SETUP  | Contains specifications of each model of chart            | Py dictionary
+                |    Dictionary tags                                        |
+                |    'NAME'          == Filename output file                | String 
+                |    'WIDTH'         == Width figure                        | Float
+                |    'HEIGHT         == Height figure                       | Float
+                |    'X AXIS SIZE'   == X axis size                         | Float
+                |    'Y AXIS SIZE'   == Y axis size                         | Float
+                |    'AXISES COLOR'  == Axis color                          | String
+                |    'X AXIS LABEL'  == X label name                        | String
+                |    'LABELS SIZE'   == Labels size                         | Float
+                |    'LABELS COLOR'  == Labels color                        | String
+                |    'CHART COLOR'   == Boxplot and histogram color         | String
+                |    'BINS'          == Range representing the width of     | Float
+                |                       a single bar                        | 
+                |    'KDE'           == Smooth of the random distribution   | Boolean      
+                |    'DPI'           == Dots Per Inch - Image quality       | Integer   
+                |    'EXTENSION'     == Extension output file               | String ('.svg, '.png', '.eps' or '.pdf')
+
+    Output:
+    The image is saved in the current directory 
+    """
+    
+	# Checking which is the best process 
+    MINVALUES = []
+    N_REP = DATASET['NUMBER OF REPETITIONS']
+    N_ITER = DATASET['NUMBER OF ITERATIONS']
+    TYPE = DATASET['OF OR FIT']
+    BEST_REP = DATASET['BEST']
+    for ID in range(N_REP):
+        if TYPE == 'OF':
+            X = BEST_REP[ID]['OF'][N_ITER]
+        else:
+            X = BEST_REP[ID]['FIT'][N_ITER]
+        MINVALUES.append(X)
+    NAME = PLOT_SETUP['NAME']
+    W = PLOT_SETUP['WIDTH']
+    H = PLOT_SETUP['HEIGHT']
+    EXT = PLOT_SETUP['EXTENSION']
+    DPI = PLOT_SETUP['DPI']
+    X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']
+    X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
+    Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']
+    AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
+    LABELS_SIZE = PLOT_SETUP['LABELS SIZE']     
+    LABELS_COLOR = PLOT_SETUP['LABELS COLOR']
+    CHART_COLOR = PLOT_SETUP['COLOR']
+    BINS = PLOT_SETUP['BINS']
+    KDE = PLOT_SETUP['KDE']
+
+    sns.set(style = 'ticks')
+
+    # Convert units of size figure
+    [W, H] = CONVERT_SI_TO_INCHES(W, H)
+    
+	# Plot
+    FIG, (AX_BOX, AX_HIST) = plt.subplots(2, figsize = (W, H), sharex = True, gridspec_kw = {'height_ratios': (.15, .85)})
+    sns.boxplot(x = MINVALUES, ax = AX_BOX, color = CHART_COLOR)
+    sns.histplot(MINVALUES, ax = AX_HIST, kde = KDE, color = CHART_COLOR, bins = BINS)
+    AX_BOX.set(yticks = [])
+    AX_BOX.set(xlabel='')
+    font = {'fontname': 'Arial',
+            'color':  LABELS_COLOR,
+            'weight': 'normal',
+            'size': LABELS_SIZE}
+    AX_HIST.set_xlabel(X_AXIS_LABEL, fontdict = font)
+    AX_HIST.set_ylabel('$Frequency$', fontdict = font)
+    AX_HIST.tick_params(axis= 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
+    AX_HIST.tick_params(axis= 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
+    sns.despine(ax = AX_HIST)
+    sns.despine(ax = AX_BOX, left = True)
+    SAVE_GRAPHIC(NAME, EXT, DPI)
+
+def META_PLOT_005(FUNCTION,X_L, X_U):
+    """
+	wsss
+	asas
+	"""
+	# Convert units of size figure
+    [W, H] = CONVERT_SI_TO_INCHES(W, H)
+	
+    N = 100
+    X_AUX = np.linspace(X_L, X_U, N)
+    Y_AUX = np.linspace(X_L, X_U, N)
+    A, B = np.meshgrid(X_AUX, Y_AUX)
+    Z = np.zeros((N,N))
+    for I in range(N):
+        for J in range(N):
+            X = [A[I, J], B[I, J]]
+            if FUNCTION == "ACKLEY":
+                Z[I, J] = META_FN.ACKLEY(X)
+            if FUNCTION == "SPHERE":
+                Z[I, J] = META_FN.SPHERE(X)
+            if FUNCTION == "ROSENBROCK":
+                Z[I, J] = META_FN.ROSENBROCK(X)
+            if FUNCTION == "RASTRIGIN":
+                Z[I, J] = META_FN.RASTRIGIN(X)
+            if FUNCTION == "GRIEWANK":
+                Z[I, J] = META_FN.GRIEWANK(X)
+            if FUNCTION == "ZAKHAROV":
+                Z[I, J] = META_FN.ZAKHAROV(X)
+            if FUNCTION == "EASOM":
+                Z[I, J] = META_FN.EASOM(X)
+            if FUNCTION == "MICHALEWICS":
+                Z[I, J] = META_FN.MICHALEWICS(X)
+    fig = plt.figure()
+    ax = plt.axes(projection = '3d')
+    ax.contour3D(A, B, Z, 100, cmap = 'jet')
+    ax.set_xlabel('x')
+    ax.set_ylabel('y')
+    ax.set_zlabel('z')
```

### Comparing `META_TOOLBOX-2023.1/META_TOOLBOX/META_HC_LIBRARY.py` & `META_TOOLBOX-2023.2/META_TOOLBOX/META_HC_LIBRARY.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import numpy as np
-import META_TOOLBOX.META_CO_LIBRARY as META_CO
-
-def HC_MOVEMENT(OF_FUNCTION, NULL_DIC, X_IOLD, X_L, X_U, D, SIGMA):
-    """ 
-    This function creates a new solution using Hill Climbing movement.
-
-    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/HC.html
-    """
-    # Start internal variables
-    X_INEW = []
-    OF_INEW = 0
-    FIT_INEW = 0
-    
-    # Particle Hill Climbing movement (Normal distribution)
-    for I in range(D):
-        MEAN_VALUE = X_IOLD[I]
-        SIGMA_VALUE = abs(MEAN_VALUE * SIGMA)
-        NEIGHBOR = np.random.normal(MEAN_VALUE, SIGMA_VALUE, 1)
-        X_INEW.append(NEIGHBOR[0])
-    
-    # Check bounds
-    X_INEW = META_CO.CHECK_INTERVAL_01(X_INEW, X_L, X_U) 
-    
-    # Evaluation of the objective function and fitness
-    OF_INEW = OF_FUNCTION(X_INEW, NULL_DIC)
-    FIT_INEW = META_CO.FIT_VALUE(OF_INEW)
-    NEOF = 1
-    
+import numpy as np
+import META_TOOLBOX.META_CO_LIBRARY as META_CO
+
+def HC_MOVEMENT(OF_FUNCTION, NULL_DIC, X_IOLD, X_L, X_U, D, SIGMA):
+    """ 
+    This function creates a new solution using Hill Climbing movement.
+
+    See documentation in https://wmpjrufg.github.io/META_TOOLBOX/HC.html
+    """
+    # Start internal variables
+    X_INEW = []
+    OF_INEW = 0
+    FIT_INEW = 0
+    
+    # Particle Hill Climbing movement (Normal distribution)
+    for I in range(D):
+        MEAN_VALUE = X_IOLD[I]
+        SIGMA_VALUE = abs(MEAN_VALUE * SIGMA)
+        NEIGHBOR = np.random.normal(MEAN_VALUE, SIGMA_VALUE, 1)
+        X_INEW.append(NEIGHBOR[0])
+    
+    # Check bounds
+    X_INEW = META_CO.CHECK_INTERVAL_01(X_INEW, X_L, X_U) 
+    
+    # Evaluation of the objective function and fitness
+    OF_INEW = OF_FUNCTION(X_INEW, NULL_DIC)
+    FIT_INEW = META_CO.FIT_VALUE(OF_INEW)
+    NEOF = 1
+    
     return X_INEW, OF_INEW, FIT_INEW, NEOF
```

### Comparing `META_TOOLBOX-2023.1/META_TOOLBOX/META_SA_LIBRARY.py` & `META_TOOLBOX-2023.2/META_TOOLBOX/META_SA_LIBRARY.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,56 @@
-import numpy as np
-import META_TOOLBOX.META_CO_LIBRARY as META_CO
-import META_TOOLBOX.META_HC_LIBRARY as META_HC
-
-def START_TEMPERATURE(OF_FUNCTION, NULL_DIC, N_POP, D, X_L, X_U, X, OF, SIGMA):
-    """ 
-    This function calculates the initial temperature in function of a probability of acceptance of 50% of the initial solutions.  
-
-    Input:
-    OF_FUNCTION        | External def user input this function in arguments           | Py function
-    N_POP              | Number of population                                         | Integer
-    D                  | Problem dimension                                            | Integer
-    X                  | Design variables                                             | Py Numpy array[N_POP x D]
-    X_L                | Lower limit design variables                                 | Py list[D]
-    X_U                | Upper limit design variables                                 | Py list[D]
-    OF                 | All objective function values                                | Py Numpy array[N_POP x 1]
-    SIGMA              | Standard deviation the normal distribution in percentage     | Float
-    TEMP               | Initial temperature or automatic temperature value that has  | Float
-                       | an 80% probability of accepting the movement of particles    |
-    STOP_CONTROL_TEMP  | Stop criteria about initial temperature try                  | Float
-                       | or automatic value = 1000                   
-        
-    Output:
-    T_INITIAL          | Initial temperature SA algorithm                             | Float
-    """
-    
-    # Atiqullah, M. M. (2004). An Efficient Simple Cooling Schedule for Simulated Annealing. Lecture Notes in Computer Science, 396–404. doi:10.1007/978-3-540-24767-8_41 
-    T_0TRIAL = []
-    TRIAL = 10
-
-    # Population movement 
-    for POP in range(N_POP):
-
-        DELTAC = []
-        
-        # Trial
-        for I in range(TRIAL):
-            
-            # Simulated Annealing particle movement (Same Hill Climbing movement)
-            X_ITEMP, OF_ITEMP, FIT_ITEMP, NEOF = META_HC.HC_MOVEMENT(OF_FUNCTION, NULL_DIC, X[POP, :], X_L, X_U, D, SIGMA) 
-
-            # Energy
-            AUX = np.abs(OF_ITEMP - OF[POP, 0])
-            DELTAC.append(AUX)
-
-        # Total energy
-        DELTAC_MEAN = np.mean(DELTAC)
-        DELTAC_STD = np.std(DELTAC)
-        
-        # Save temperature
-        AUX = - (DELTAC_MEAN + 3 * DELTAC_STD) / np.log(0.5)
-        T_0TRIAL.append(AUX)
-
-    # Initital temperature
-    T_0 = np.max(T_0TRIAL)
-    
+import numpy as np
+import META_TOOLBOX.META_HC_LIBRARY as META_HC
+
+def START_TEMPERATURE(OF_FUNCTION, NULL_DIC, N_POP, D, X_L, X_U, X, OF, SIGMA):
+    """ 
+    This function calculates the initial temperature in function of a probability of acceptance of 50% of the initial solutions.  
+
+    Input:
+    OF_FUNCTION        | External def user input this function in arguments           | Py function
+    N_POP              | Number of population                                         | Integer
+    D                  | Problem dimension                                            | Integer
+    X                  | Design variables                                             | Py Numpy array[N_POP x D]
+    X_L                | Lower limit design variables                                 | Py list[D]
+    X_U                | Upper limit design variables                                 | Py list[D]
+    OF                 | All objective function values                                | Py Numpy array[N_POP x 1]
+    SIGMA              | Standard deviation the normal distribution in percentage     | Float
+    TEMP               | Initial temperature or automatic temperature value that has  | Float
+                       | an 80% probability of accepting the movement of particles    |
+    STOP_CONTROL_TEMP  | Stop criteria about initial temperature try                  | Float
+                       | or automatic value = 1000                   
+        
+    Output:
+    T_INITIAL          | Initial temperature SA algorithm                             | Float
+    """
+    
+    # Atiqullah, M. M. (2004). An Efficient Simple Cooling Schedule for Simulated Annealing. Lecture Notes in Computer Science, 396–404. doi:10.1007/978-3-540-24767-8_41 
+    T_0TRIAL = []
+    TRIAL = 10
+
+    # Population movement 
+    for POP in range(N_POP):
+
+        DELTAC = []
+        
+        # Trial
+        for I in range(TRIAL):
+            
+            # Simulated Annealing particle movement (Same Hill Climbing movement)
+            X_ITEMP, OF_ITEMP, FIT_ITEMP, NEOF = META_HC.HC_MOVEMENT(OF_FUNCTION, NULL_DIC, X[POP, :], X_L, X_U, D, SIGMA) 
+
+            # Energy
+            AUX = np.abs(OF_ITEMP - OF[POP, 0])
+            DELTAC.append(AUX)
+
+        # Total energy
+        DELTAC_MEAN = np.mean(DELTAC)
+        DELTAC_STD = np.std(DELTAC)
+        
+        # Save temperature
+        AUX = - (DELTAC_MEAN + 3 * DELTAC_STD) / np.log(0.5)
+        T_0TRIAL.append(AUX)
+
+    # Initital temperature
+    T_0 = np.max(T_0TRIAL)
+    
     return T_0
```

### Comparing `META_TOOLBOX-2023.1/META_TOOLBOX.egg-info/PKG-INFO` & `META_TOOLBOX-2023.2/META_TOOLBOX.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 1.1
-Name: META-TOOLBOX
-Version: 2023.1
-Summary: The METApy optimization toolbox is an easy of use environment for applying metaheuristic optimization methods. The platform has several optimization methods, as well as functions for generating charts and statistical analysis of the results.
-Home-page: https://wmpjrufg.github.io/META_TOOLBOX/
-Author: UNKNOWN
-Author-email: wanderlei_junior@ufcat.edu.br
-License: Apache License
-Description: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering
+Metadata-Version: 2.1
+Name: META-TOOLBOX
+Version: 2023.2
+Summary: The METApy optimization toolbox is an easy of use environment for applying metaheuristic optimization methods. The platform has several optimization methods, as well as functions for generating charts and statistical analysis of the results.
+Home-page: https://wmpjrufg.github.io/META_TOOLBOX/
+Author-email: wanderlei_junior@ufcat.edu.br
+License: Apache License
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `META_TOOLBOX-2023.1/PKG-INFO` & `META_TOOLBOX-2023.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 1.1
-Name: META_TOOLBOX
-Version: 2023.1
-Summary: The METApy optimization toolbox is an easy of use environment for applying metaheuristic optimization methods. The platform has several optimization methods, as well as functions for generating charts and statistical analysis of the results.
-Home-page: https://wmpjrufg.github.io/META_TOOLBOX/
-Author: UNKNOWN
-Author-email: wanderlei_junior@ufcat.edu.br
-License: Apache License
-Description: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering
+Metadata-Version: 2.1
+Name: META_TOOLBOX
+Version: 2023.2
+Summary: The METApy optimization toolbox is an easy of use environment for applying metaheuristic optimization methods. The platform has several optimization methods, as well as functions for generating charts and statistical analysis of the results.
+Home-page: https://wmpjrufg.github.io/META_TOOLBOX/
+Author-email: wanderlei_junior@ufcat.edu.br
+License: Apache License
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `META_TOOLBOX-2023.1/README.md` & `META_TOOLBOX-2023.2/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# pacotepypi
-Example of PyPI package.
-## Getting Started
-#### Dependencies
-You need Python 3.7 or later to use **pacotepypi**. You can find it at [python.org](https://www.python.org/).
-You also need setuptools, wheel and twine packages, which is available from [PyPI](https://pypi.org). If you have pip, just run:
-```
-pip install setuptools
-pip install wheel
-pip install twine
-```
-#### Installation
-Clone this repo to your local machine using:
-```
-git clone https://github.com/caiocarneloz/pacotepypi.git
-```
-## Features
-- File structure for PyPI packages
-- Setup with package informations
+# pacotepypi
+Example of PyPI package.
+## Getting Started
+#### Dependencies
+You need Python 3.7 or later to use **pacotepypi**. You can find it at [python.org](https://www.python.org/).
+You also need setuptools, wheel and twine packages, which is available from [PyPI](https://pypi.org). If you have pip, just run:
+```
+pip install setuptools
+pip install wheel
+pip install twine
+```
+#### Installation
+Clone this repo to your local machine using:
+```
+git clone https://github.com/caiocarneloz/pacotepypi.git
+```
+## Features
+- File structure for PyPI packages
+- Setup with package informations
 - License example
```

### Comparing `META_TOOLBOX-2023.1/setup.py` & `META_TOOLBOX-2023.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from setuptools import setup
-
-setup(
-    	name = 'META_TOOLBOX',
-    	version = '2023.1',
-		url='https://wmpjrufg.github.io/META_TOOLBOX/',
-    	license='Apache License',
-    	author_email = 'wanderlei_junior@ufcat.edu.br',
-    	packages = ['META_TOOLBOX'],
-    	description = "The METApy optimization toolbox is an easy of use environment for applying metaheuristic optimization methods. The platform has several optimization methods, as well as functions for generating charts and statistical analysis of the results.",
-    	classifiers = ["Programming Language :: Python","Topic :: Scientific/Engineering :: Mathematics", "Topic :: Scientific/Engineering"],
-    	install_requires = ["Numpy", "Xlsxwriter"]
-    )
-
+from setuptools import setup
+
+setup(
+    	name = 'META_TOOLBOX',
+    	version = '2023.2',
+		url = 'https://wmpjrufg.github.io/META_TOOLBOX/',
+    	license = 'Apache License',
+    	author_email = 'wanderlei_junior@ufcat.edu.br',
+    	packages = ['META_TOOLBOX'],
+    	description = "The METApy optimization toolbox is an easy of use environment for applying metaheuristic optimization methods. The platform has several optimization methods, as well as functions for generating charts and statistical analysis of the results.",
+    	classifiers = ["Programming Language :: Python","Topic :: Scientific/Engineering :: Mathematics", "Topic :: Scientific/Engineering"],
+    	install_requires = ["Numpy", "Xlsxwriter", "pandas"]
+    )
+
```


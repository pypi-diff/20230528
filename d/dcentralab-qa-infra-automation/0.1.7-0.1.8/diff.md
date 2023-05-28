# Comparing `tmp/dcentralab_qa_infra_automation-0.1.7.tar.gz` & `tmp/dcentralab_qa_infra_automation-0.1.8.tar.gz`

## Comparing `dcentralab_qa_infra_automation-0.1.7.tar` & `dcentralab_qa_infra_automation-0.1.8.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/.idea/packaging.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/.idea/vcs.xml
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/.idea/workspace.xml
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/__init__.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/data/read_data.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/BasePage.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
--rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/LICENSE
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/.idea/packaging.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/.idea/vcs.xml
+-rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/.idea/workspace.xml
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/__init__.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/data/read_data.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/BasePage.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
+-rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/LICENSE
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.8/PKG-INFO
```

### Comparing `dcentralab_qa_infra_automation-0.1.7/.idea/workspace.xml` & `dcentralab_qa_infra_automation-0.1.8/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `dcentralab_qa_infra_automation-0.1.7/.idea/workspace.xml` & `dcentralab_qa_infra_automation-0.1.8/.idea/workspace.xml`

```diff
@@ -2,14 +2,15 @@
 <project version="4">
   <component name="ChangeListManager">
     <list default="true" id="ce720036-d8eb-462b-9d8d-e560b75fc3e8" name="Changes" comment="change package name">
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/__init__.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/BasePage.py" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py" afterDir="false"/>
@@ -57,24 +58,24 @@
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
-    "last_opened_file_path": "C:/Users/Efrat Cohen/Desktop/projects/packaging/src/dcentralab_qa_infra_automation"
+    "last_opened_file_path": "C:/Users/Efrat Cohen/Desktop/projects/packaging/src/dcentralab_qa_infra_automation/pages/coinbasePages"
   }
 }]]></component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
+      <recent name="C:\Users\Efrat Cohen\Desktop\projects\packaging\src\dcentralab_qa_infra_automation\pages\coinbasePages"/>
       <recent name="C:\Users\Efrat Cohen\Desktop\projects\packaging\src\dcentralab_qa_infra_automation"/>
       <recent name="C:\Users\Efrat Cohen\Desktop\projects\packaging\src\dcentralab_qa_infra_automation\fixtures"/>
       <recent name="C:\Users\Efrat Cohen\Desktop\projects\packaging\src\dcentralab_qa_infra_automation\drivers"/>
       <recent name="C:\Users\Efrat Cohen\Desktop\projects\packaging\src\seleniumPythonFramework_VeriSoft"/>
-      <recent name="C:\Users\Efrat Cohen\Desktop\projects\packaging"/>
     </key>
     <key name="MoveFile.RECENT_KEYS">
       <recent name="C:\Users\Efrat Cohen\Desktop\projects\packaging\src\seleniumPythonFramework_VeriSoft\files"/>
     </key>
   </component>
   <component name="RunManager">
     <configuration name="main" type="PythonConfigurationType" factoryName="Python" nameIsGenerated="true">
```

### Comparing `dcentralab_qa_infra_automation-0.1.7/.idea/inspectionProfiles/Project_Default.xml` & `dcentralab_qa_infra_automation-0.1.8/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/data/read_data.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/data/read_data.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/Loggers.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/Loggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/BasePage.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/BasePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import time
 
 import pytest
 from dcentralab_qa_infra_automation.utils.WalletsActionsInterface import WalletsActionsInterface
+
+from dcentralab_qa_infra_automation.pages.coinbasePages.ConnectToWebsitePage import ConnectToWebsitePage
 from dcentralab_qa_infra_automation.pages.coinbasePages.CreatePasswordPage import CreatePasswordPage
 from dcentralab_qa_infra_automation.pages.coinbasePages.CreateWalletPage import CreateWalletPage
 from dcentralab_qa_infra_automation.pages.coinbasePages.ImportWalletPage import ImportWalletPage
 from dcentralab_qa_infra_automation.pages.coinbasePages.ReceiveCryptoToUsername import ReceiveCryptoToUsernamePage
 from dcentralab_qa_infra_automation.pages.coinbasePages.UseAnExistingWalletPage import UseAnExistingWalletPage
+from dcentralab_qa_infra_automation.pages.coinbasePages.ConfirmPage import ConfirmPage
 
 
 class CoinbaseActions(WalletsActionsInterface):
     """
     coinbase actions class
     this class implements wallet actions interface.
     """
@@ -86,8 +89,61 @@
 
         # Switch focus to first tab
         self.driver.switch_to.window(self.driver.window_handles[0])
 
     def connect_wallet(self):
         """
             connect to wallet implementation
-        """
+        """
+        time.sleep(8)
+
+        # Coinbase popup instance
+        whandle = self.driver.window_handles[1]
+
+        # Switch to pop up window
+        self.driver.switch_to.window(whandle)
+
+        connectToWebsitePage = ConnectToWebsitePage(self.driver)
+
+        # Check is connect to website popup loaded
+        assert connectToWebsitePage.is_page_loaded()
+
+        # Click on connect button
+        connectToWebsitePage.click_on_connect_button()
+
+        time.sleep(2)
+
+        # Switch focus to site tab
+        self.driver.switch_to.window(self.driver.window_handles[0])
+
+    def confirm(self):
+        time.sleep(5)
+
+        # Coinbase popup instance
+        whandle = self.driver.window_handles[1]
+
+        # Switch to pop up window
+        self.driver.switch_to.window(whandle)
+
+        confirmPage = ConfirmPage(self.driver)
+
+        # Check is confirm port token page loaded
+        assert confirmPage.is_page_loaded(), "confirm port token page loaded"
+
+        # Check is got it button exist
+        assert confirmPage.is_got_it_button_exist()
+
+        # Click on got_it button
+        confirmPage.click_on_got_it_button()
+
+        time.sleep(3)
+
+        # Check is confirm button exist.
+        assert confirmPage.is_confirm_button_exist()
+
+        # Click on confirm button
+        confirmPage.click_on_confirm_button()
+
+        time.sleep(5)
+
+        # Switch focus to site tab
+        self.driver.switch_to.window(self.driver.window_handles[0])
```

### Comparing `dcentralab_qa_infra_automation-0.1.7/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py` & `dcentralab_qa_infra_automation-0.1.8/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/LICENSE` & `dcentralab_qa_infra_automation-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.7/pyproject.toml` & `dcentralab_qa_infra_automation-0.1.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcentralab_qa_infra_automation"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Efrat Cohen", email="efrat.cohen@verisoft.co" },
 ]
 description = "Selenium Python Framework developed by veriSoft"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dcentralab_qa_infra_automation-0.1.7/PKG-INFO` & `dcentralab_qa_infra_automation-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentralab_qa_infra_automation
-Version: 0.1.7
+Version: 0.1.8
 Summary: Selenium Python Framework developed by veriSoft
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Efrat Cohen <efrat.cohen@verisoft.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


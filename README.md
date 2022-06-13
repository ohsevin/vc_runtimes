# vc_runtimes

visual studio c++ runtimes (all architectures).  

- installable (double click msi)
- embeddable (you can use standard administrator embedding).
- copyable (you can just copy the file to a folder of a programs that requires it).

- unpacked from wix exe container  
using the wix toolset https://wixtoolset.org/releases/  
with `dark.exe myinstaller.exe -x "C:...target-dir..."`

- archived msi files were unpacked as well  
with `msiexec.exe /a archive.msi /qb /l log.txt TARGETDIR="C:...target-dir..."`  
you can still use the msi for both installation (just double click it),  
and embedding, just keep the folder structure. the msi is just an installation script now..

- folder structure simplified.

- this thing is unofficial, but files are unmodified, all of them are Microsoft signed.

- repository last updated: June 2022.

<br/>
<hr/>

<details><summary>this is the structure of the repository (folders and files)</summary>

```txt
/
|   .gitattributes
|   README.md
|   Visual Studio 2008 (VC++ 9.0) SP1 (no longer supported) vcredist_x64_extracted.zip
|   Visual Studio 2008 (VC++ 9.0) SP1 (no longer supported) vcredist_x86_extracted.zip
|   Visual Studio 2010 (VC++ 10.0) SP1 (no longer supported) vcredist_x64_extracted.zip
|   Visual Studio 2010 (VC++ 10.0) SP1 (no longer supported) vcredist_x86_extracted.zip
|   Visual Studio 2012 (VC++ 11.0) Update 4 vcredist_x64_extracted.zip
|   Visual Studio 2012 (VC++ 11.0) Update 4 vcredist_x86_extracted.zip
|   Visual Studio 2013 (VC++ 12.0) vcredist_x64_extracted.zip
|   Visual Studio 2013 (VC++ 12.0) vcredist_x86_extracted.zip
|   Visual Studio 2015, 2017, 2019, and 2022 VC_redist.arm64_extracted.zip
|   Visual Studio 2015, 2017, 2019, and 2022 VC_redist.x64_extracted.zip
|   Visual Studio 2015, 2017, 2019, and 2022 VC_redist.x86_extracted.zip
|   
+---Visual Studio 2008 (VC++ 9.0) SP1 (no longer supported) vcredist_x64_extracted
|   |   eula.1028.txt
|   |   eula.1031.txt
|   |   eula.1033.txt
|   |   eula.1036.txt
|   |   eula.1040.txt
|   |   eula.1041.txt
|   |   eula.1042.txt
|   |   eula.1049.txt
|   |   eula.2052.txt
|   |   eula.3082.txt
|   |   globdata.ini
|   |   install.exe
|   |   install.ini
|   |   install.res.1028.dll
|   |   install.res.1031.dll
|   |   install.res.1033.dll
|   |   install.res.1036.dll
|   |   install.res.1040.dll
|   |   install.res.1041.dll
|   |   install.res.1042.dll
|   |   install.res.1049.dll
|   |   install.res.2052.dll
|   |   install.res.3082.dll
|   |   vcredist.bmp
|   |   VC_RED.cab
|   |   VC_RED.MSI
|   |   
|   +---Program Files(64)
|   |   \---Common Files
|   |       \---Microsoft Shared
|   |           \---VC
|   |                   msdia90.dll
|   |                   
|   \---Windows
|       \---winsxs
|           +---dlATLx64
|           |       atl90.dll
|           |       
|           +---dlCRTx64
|           |       msvcm90.dll
|           |       msvcp90.dll
|           |       msvcr90.dll
|           |       
|           +---dlMFCLOCx64
|           |       mfc90chs.dll
|           |       mfc90cht.dll
|           |       mfc90deu.dll
|           |       mfc90enu.dll
|           |       mfc90esn.dll
|           |       mfc90esp.dll
|           |       mfc90fra.dll
|           |       mfc90ita.dll
|           |       mfc90jpn.dll
|           |       mfc90kor.dll
|           |       mfc90rus.dll
|           |       
|           +---dlMFCx64
|           |       mfc90.dll
|           |       mfc90u.dll
|           |       mfcm90.dll
|           |       mfcm90u.dll
|           |       
|           +---dlOpenMPx64
|           |       vcomp90.dll
|           |       
|           +---Manifests
|           |       amd64_Microsoft.VC90.ATL_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_c44f2197.cat
|           |       amd64_Microsoft.VC90.ATL_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_c44f2197.manifest
|           |       amd64_Microsoft.VC90.CRT_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_63af3423.cat
|           |       amd64_Microsoft.VC90.CRT_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_63af3423.manifest
|           |       amd64_Microsoft.VC90.MFCLOC_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_a5161ae8.cat
|           |       amd64_Microsoft.VC90.MFCLOC_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_a5161ae8.manifest
|           |       amd64_Microsoft.VC90.MFC_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_3495a728.cat
|           |       amd64_Microsoft.VC90.MFC_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_3495a728.manifest
|           |       amd64_Microsoft.VC90.OpenMP_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_7fe65c7f.cat
|           |       amd64_Microsoft.VC90.OpenMP_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_7fe65c7f.manifest
|           |       
|           +---Policies
|           |   +---dlpATLx64
|           |   |       9.0.30729.6161.cat
|           |   |       9.0.30729.6161.policy
|           |   |       
|           |   +---dlpCRTx64
|           |   |       9.0.30729.6161.cat
|           |   |       9.0.30729.6161.policy
|           |   |       
|           |   +---dlpMFCLOCx64
|           |   |       9.0.30729.6161.cat
|           |   |       9.0.30729.6161.policy
|           |   |       
|           |   +---dlpMFCx64
|           |   |       9.0.30729.6161.cat
|           |   |       9.0.30729.6161.policy
|           |   |       
|           |   \---dlpOpenMPx64
|           |           9.0.30729.6161.cat
|           |           9.0.30729.6161.policy
|           |           
|           +---ulATLx64
|           |       amd64_Microsoft.VC90.ATL_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_c44f2197.cat
|           |       amd64_Microsoft.VC90.ATL_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_c44f2197.manifest
|           |       atl90.dll
|           |       
|           +---ulCRTx64
|           |       amd64_Microsoft.VC90.CRT_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_63af3423.cat
|           |       amd64_Microsoft.VC90.CRT_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_63af3423.manifest
|           |       msvcm90.dll
|           |       msvcp90.dll
|           |       msvcr90.dll
|           |       
|           +---ulMFCLOCx64
|           |       amd64_Microsoft.VC90.MFCLOC_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_a5161ae8.cat
|           |       amd64_Microsoft.VC90.MFCLOC_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_a5161ae8.manifest
|           |       mfc90chs.dll
|           |       mfc90cht.dll
|           |       mfc90deu.dll
|           |       mfc90enu.dll
|           |       mfc90esn.dll
|           |       mfc90esp.dll
|           |       mfc90fra.dll
|           |       mfc90ita.dll
|           |       mfc90jpn.dll
|           |       mfc90kor.dll
|           |       mfc90rus.dll
|           |       
|           +---ulMFCx64
|           |       amd64_Microsoft.VC90.MFC_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_3495a728.cat
|           |       amd64_Microsoft.VC90.MFC_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_3495a728.manifest
|           |       mfc90.dll
|           |       mfc90u.dll
|           |       mfcm90.dll
|           |       mfcm90u.dll
|           |       
|           +---ulOpenMPx64
|           |       amd64_Microsoft.VC90.OpenMP_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_7fe65c7f.cat
|           |       amd64_Microsoft.VC90.OpenMP_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_7fe65c7f.manifest
|           |       vcomp90.dll
|           |       
|           +---ulpATLx64
|           |       9.0.30729.6161.cat
|           |       9.0.30729.6161.policy
|           |       
|           +---ulpCRTx64
|           |       9.0.30729.6161.cat
|           |       9.0.30729.6161.policy
|           |       
|           +---ulpMFCLOCx64
|           |       9.0.30729.6161.cat
|           |       9.0.30729.6161.policy
|           |       
|           +---ulpMFCx64
|           |       9.0.30729.6161.cat
|           |       9.0.30729.6161.policy
|           |       
|           \---ulpOpenMPx64
|                   9.0.30729.6161.cat
|                   9.0.30729.6161.policy
|                   
+---Visual Studio 2008 (VC++ 9.0) SP1 (no longer supported) vcredist_x86_extracted
|   |   eula.1028.txt
|   |   eula.1031.txt
|   |   eula.1033.txt
|   |   eula.1036.txt
|   |   eula.1040.txt
|   |   eula.1041.txt
|   |   eula.1042.txt
|   |   eula.1049.txt
|   |   eula.2052.txt
|   |   eula.3082.txt
|   |   globdata.ini
|   |   install.exe
|   |   install.ini
|   |   install.res.1028.dll
|   |   install.res.1031.dll
|   |   install.res.1033.dll
|   |   install.res.1036.dll
|   |   install.res.1040.dll
|   |   install.res.1041.dll
|   |   install.res.1042.dll
|   |   install.res.1049.dll
|   |   install.res.2052.dll
|   |   install.res.3082.dll
|   |   vcredist.bmp
|   |   VC_RED.cab
|   |   VC_RED.MSI
|   |   
|   +---Program Files
|   |   \---Common Files
|   |       \---Microsoft Shared
|   |           \---VC
|   |                   msdia90.dll
|   |                   
|   \---Windows
|       +---system32
|       |       atl90.dll
|       |       mfc90.dll
|       |       mfc90chs.dll
|       |       mfc90cht.dll
|       |       mfc90deu.dll
|       |       mfc90enu.dll
|       |       mfc90esn.dll
|       |       mfc90esp.dll
|       |       mfc90fra.dll
|       |       mfc90ita.dll
|       |       mfc90jpn.dll
|       |       mfc90kor.dll
|       |       mfc90rus.dll
|       |       mfc90u.dll
|       |       mfcm90.dll
|       |       mfcm90u.dll
|       |       msvcm90.dll
|       |       msvcp90.dll
|       |       msvcr90.dll
|       |       vcomp90.dll
|       |       
|       \---winsxs
|           +---dlATLx86
|           |       atl90.dll
|           |       
|           +---dlCRTx86
|           |       msvcm90.dll
|           |       msvcp90.dll
|           |       msvcr90.dll
|           |       
|           +---dlMFCLOCx86
|           |       mfc90chs.dll
|           |       mfc90cht.dll
|           |       mfc90deu.dll
|           |       mfc90enu.dll
|           |       mfc90esn.dll
|           |       mfc90esp.dll
|           |       mfc90fra.dll
|           |       mfc90ita.dll
|           |       mfc90jpn.dll
|           |       mfc90kor.dll
|           |       mfc90rus.dll
|           |       
|           +---dlMFCx86
|           |       mfc90.dll
|           |       mfc90u.dll
|           |       mfcm90.dll
|           |       mfcm90u.dll
|           |       
|           +---dlOpenMPx86
|           |       vcomp90.dll
|           |       
|           +---Manifests
|           |       x86_Microsoft.VC90.ATL_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_92453bb7.cat
|           |       x86_Microsoft.VC90.ATL_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_92453bb7.manifest
|           |       x86_Microsoft.VC90.CRT_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_31a54e43.cat
|           |       x86_Microsoft.VC90.CRT_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_31a54e43.manifest
|           |       x86_Microsoft.VC90.MFCLOC_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_730c3508.cat
|           |       x86_Microsoft.VC90.MFCLOC_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_730c3508.manifest
|           |       x86_Microsoft.VC90.MFC_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_028bc148.cat
|           |       x86_Microsoft.VC90.MFC_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_028bc148.manifest
|           |       x86_Microsoft.VC90.OpenMP_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_4ddc769f.cat
|           |       x86_Microsoft.VC90.OpenMP_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_4ddc769f.manifest
|           |       
|           +---Policies
|           |   +---dlpATLx86
|           |   |       9.0.30729.6161.cat
|           |   |       9.0.30729.6161.policy
|           |   |       
|           |   +---dlpCRTx86
|           |   |       9.0.30729.6161.cat
|           |   |       9.0.30729.6161.policy
|           |   |       
|           |   +---dlpMFCLOCx86
|           |   |       9.0.30729.6161.cat
|           |   |       9.0.30729.6161.policy
|           |   |       
|           |   +---dlpMFCx86
|           |   |       9.0.30729.6161.cat
|           |   |       9.0.30729.6161.policy
|           |   |       
|           |   \---dlpOpenMPx86
|           |           9.0.30729.6161.cat
|           |           9.0.30729.6161.policy
|           |           
|           +---ulATLx86
|           |       atl90.dll
|           |       x86_Microsoft.VC90.ATL_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_92453bb7.cat
|           |       x86_Microsoft.VC90.ATL_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_92453bb7.manifest
|           |       
|           +---ulCRTx86
|           |       msvcm90.dll
|           |       msvcp90.dll
|           |       msvcr90.dll
|           |       x86_Microsoft.VC90.CRT_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_31a54e43.cat
|           |       x86_Microsoft.VC90.CRT_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_31a54e43.manifest
|           |       
|           +---ulMFCLOCx86
|           |       mfc90chs.dll
|           |       mfc90cht.dll
|           |       mfc90deu.dll
|           |       mfc90enu.dll
|           |       mfc90esn.dll
|           |       mfc90esp.dll
|           |       mfc90fra.dll
|           |       mfc90ita.dll
|           |       mfc90jpn.dll
|           |       mfc90kor.dll
|           |       mfc90rus.dll
|           |       x86_Microsoft.VC90.MFCLOC_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_730c3508.cat
|           |       x86_Microsoft.VC90.MFCLOC_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_730c3508.manifest
|           |       
|           +---ulMFCx86
|           |       mfc90.dll
|           |       mfc90u.dll
|           |       mfcm90.dll
|           |       mfcm90u.dll
|           |       x86_Microsoft.VC90.MFC_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_028bc148.cat
|           |       x86_Microsoft.VC90.MFC_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_028bc148.manifest
|           |       
|           +---ulOpenMPx86
|           |       vcomp90.dll
|           |       x86_Microsoft.VC90.OpenMP_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_4ddc769f.cat
|           |       x86_Microsoft.VC90.OpenMP_1fc8b3b9a1e18e3b_9.0.30729.6161_x-ww_4ddc769f.manifest
|           |       
|           +---ulpATLx86
|           |       9.0.30729.6161.cat
|           |       9.0.30729.6161.policy
|           |       
|           +---ulpCRTx86
|           |       9.0.30729.6161.cat
|           |       9.0.30729.6161.policy
|           |       
|           +---ulpMFCLOCx86
|           |       9.0.30729.6161.cat
|           |       9.0.30729.6161.policy
|           |       
|           +---ulpMFCx86
|           |       9.0.30729.6161.cat
|           |       9.0.30729.6161.policy
|           |       
|           \---ulpOpenMPx86
|                   9.0.30729.6161.cat
|                   9.0.30729.6161.policy
|                   
+---Visual Studio 2010 (VC++ 10.0) SP1 (no longer supported) vcredist_x64_extracted
|   |   vc_red.msi
|   |   
|   \---Win
|       \---System64
|               atl100.dll
|               mfc100.dll
|               mfc100chs.dll
|               mfc100cht.dll
|               mfc100deu.dll
|               mfc100enu.dll
|               mfc100esn.dll
|               mfc100fra.dll
|               mfc100ita.dll
|               mfc100jpn.dll
|               mfc100kor.dll
|               mfc100rus.dll
|               mfc100u.dll
|               mfcm100.dll
|               mfcm100u.dll
|               msvcp100.dll
|               msvcr100.dll
|               vcomp100.dll
|               
+---Visual Studio 2010 (VC++ 10.0) SP1 (no longer supported) vcredist_x86_extracted
|   |   vc_red.msi
|   |   
|   \---Win
|       \---System
|               atl100.dll
|               mfc100.dll
|               mfc100chs.dll
|               mfc100cht.dll
|               mfc100deu.dll
|               mfc100enu.dll
|               mfc100esn.dll
|               mfc100fra.dll
|               mfc100ita.dll
|               mfc100jpn.dll
|               mfc100kor.dll
|               mfc100rus.dll
|               mfc100u.dll
|               mfcm100.dll
|               mfcm100u.dll
|               msvcp100.dll
|               msvcr100.dll
|               vcomp100.dll
|               
+---Visual Studio 2012 (VC++ 11.0) Update 4 vcredist_x64_extracted
|   +---vc_runtimeAdditional_x64
|   |   |   vc_runtimeAdditional_x64.msi
|   |   |   
|   |   \---Win
|   |       \---System64
|   |               mfc110.dll
|   |               mfc110chs.dll
|   |               mfc110cht.dll
|   |               mfc110deu.dll
|   |               mfc110enu.dll
|   |               mfc110esn.dll
|   |               mfc110fra.dll
|   |               mfc110ita.dll
|   |               mfc110jpn.dll
|   |               mfc110kor.dll
|   |               mfc110rus.dll
|   |               mfc110u.dll
|   |               mfcm110.dll
|   |               mfcm110u.dll
|   |               vcamp110.dll
|   |               vcomp110.dll
|   |               
|   \---vc_runtimeMinimum_x64
|       |   vc_runtimeMinimum_x64.msi
|       |   
|       \---Win
|           \---System64
|                   atl110.dll
|                   msvcp110.dll
|                   msvcr110.dll
|                   vccorlib110.dll
|                   
+---Visual Studio 2012 (VC++ 11.0) Update 4 vcredist_x86_extracted
|   +---vc_runtimeAdditional_x86
|   |   |   vc_runtimeAdditional_x86.msi
|   |   |   
|   |   \---Win
|   |       \---System
|   |               mfc110.dll
|   |               mfc110chs.dll
|   |               mfc110cht.dll
|   |               mfc110deu.dll
|   |               mfc110enu.dll
|   |               mfc110esn.dll
|   |               mfc110fra.dll
|   |               mfc110ita.dll
|   |               mfc110jpn.dll
|   |               mfc110kor.dll
|   |               mfc110rus.dll
|   |               mfc110u.dll
|   |               mfcm110.dll
|   |               mfcm110u.dll
|   |               vcamp110.dll
|   |               vcomp110.dll
|   |               
|   \---vc_runtimeMinimum_x86
|       |   vc_runtimeMinimum_x86.msi
|       |   
|       \---Win
|           \---System
|                   atl110.dll
|                   msvcp110.dll
|                   msvcr110.dll
|                   vccorlib110.dll
|                   
+---Visual Studio 2013 (VC++ 12.0) vcredist_x64_extracted
|   +---vc_runtimeAdditional_x64
|   |   |   vc_runtimeAdditional_x64.msi
|   |   |   
|   |   \---System64
|   |           mfc120.dll
|   |           mfc120chs.dll
|   |           mfc120cht.dll
|   |           mfc120deu.dll
|   |           mfc120enu.dll
|   |           mfc120esn.dll
|   |           mfc120fra.dll
|   |           mfc120ita.dll
|   |           mfc120jpn.dll
|   |           mfc120kor.dll
|   |           mfc120rus.dll
|   |           mfc120u.dll
|   |           mfcm120.dll
|   |           mfcm120u.dll
|   |           
|   \---vc_runtimeMinimum_x64
|       |   vc_runtimeMinimum_x64.msi
|       |   
|       \---System64
|               msvcp120.dll
|               msvcr120.dll
|               vcamp120.dll
|               vccorlib120.dll
|               vcomp120.dll
|               
+---Visual Studio 2013 (VC++ 12.0) vcredist_x86_extracted
|   +---vc_runtimeAdditional_x86
|   |   |   vc_runtimeAdditional_x86.msi
|   |   |   
|   |   \---System
|   |           mfc120.dll
|   |           mfc120chs.dll
|   |           mfc120cht.dll
|   |           mfc120deu.dll
|   |           mfc120enu.dll
|   |           mfc120esn.dll
|   |           mfc120fra.dll
|   |           mfc120ita.dll
|   |           mfc120jpn.dll
|   |           mfc120kor.dll
|   |           mfc120rus.dll
|   |           mfc120u.dll
|   |           mfcm120.dll
|   |           mfcm120u.dll
|   |           
|   \---vc_runtimeMinimum_x86
|       |   vc_runtimeMinimum_x86.msi
|       |   
|       \---System
|               msvcp120.dll
|               msvcr120.dll
|               vcamp120.dll
|               vccorlib120.dll
|               vcomp120.dll
|               
+---Visual Studio 2015, 2017, 2019, and 2022 VC_redist.arm64_extracted
|   \---VC_Runtime_arm64
|       |   VC_Runtime_arm64.msi
|       |   
|       \---System64
|               concrt140.dll
|               mfc140.dll
|               mfc140chs.dll
|               mfc140cht.dll
|               mfc140deu.dll
|               mfc140enu.dll
|               mfc140esn.dll
|               mfc140fra.dll
|               mfc140ita.dll
|               mfc140jpn.dll
|               mfc140kor.dll
|               mfc140rus.dll
|               mfc140u.dll
|               msvcp140.dll
|               msvcp140_1.dll
|               msvcp140_2.dll
|               msvcp140_atomic_wait.dll
|               msvcp140_codecvt_ids.dll
|               vcamp140.dll
|               vccorlib140.dll
|               vcomp140.dll
|               vcruntime140.dll
|               vcruntime140_1.dll
|               
+---Visual Studio 2015, 2017, 2019, and 2022 VC_redist.x64_extracted
|   +---Patch
|   |   +---x64
|   |   |   +---_Windows6.0-KB2999226-x64.msu_
|   |   |   |   +---JUNK
|   |   |   |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_1_for_kb2999226~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_1_for_kb2999226~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_2_for_kb2999226~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_2_for_kb2999226~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_3_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_3_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_3_for_kb2999226~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_3_for_kb2999226~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_for_kb2999226_client_2_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_for_kb2999226_client_2_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_for_kb2999226_client_2~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_for_kb2999226_client_2~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_for_kb2999226_client_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_for_kb2999226_client_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_for_kb2999226_client~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_for_kb2999226_client~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_for_kb2999226_sc_1_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_for_kb2999226_sc_1_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_for_kb2999226_sc_1~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_for_kb2999226_sc_1~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_for_kb2999226_sc_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_for_kb2999226_sc_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_for_kb2999226_sc~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_for_kb2999226_sc~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_for_kb2999226_server_1_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_for_kb2999226_server_1_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_for_kb2999226_server_1~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_for_kb2999226_server_1~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_for_kb2999226_server_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_for_kb2999226_server_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       package_for_kb2999226_server~31bf3856ad364e35~amd64~~6.0.1.6.cat
|   |   |   |   |       package_for_kb2999226_server~31bf3856ad364e35~amd64~~6.0.1.6.mum
|   |   |   |   |       update-bf.cat
|   |   |   |   |       update-bf.mum
|   |   |   |   |       update.cat
|   |   |   |   |       update.mum
|   |   |   |   |       
|   |   |   |   +---MSIL
|   |   |   |   +---PATCH
|   |   |   |   |       Windows6.0-KB2999226-x64-pkgProperties.txt
|   |   |   |   |       Windows6.0-KB2999226-x64.cab
|   |   |   |   |       Windows6.0-KB2999226-x64.xml
|   |   |   |   |       WSUSSCAN.cab
|   |   |   |   |       
|   |   |   |   +---WOW64
|   |   |   |   +---x64
|   |   |   |   |   +---u..salcrt-apifwd-vista_6.0.6002.19488
|   |   |   |   |   |       api-ms-win-core-console-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-datetime-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-debug-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-errorhandling-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-file-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-file-l1-2-0.dll
|   |   |   |   |   |       api-ms-win-core-file-l2-1-0.dll
|   |   |   |   |   |       api-ms-win-core-handle-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-heap-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-interlocked-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-libraryloader-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-localization-l1-2-0.dll
|   |   |   |   |   |       api-ms-win-core-memory-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-namedpipe-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-profile-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-rtlsupport-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-string-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-synch-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-synch-l1-2-0.dll
|   |   |   |   |   |       api-ms-win-core-sysinfo-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-timezone-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-util-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-xstate-l2-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-conio-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-convert-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-environment-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-heap-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-locale-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-math-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-private-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-process-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-runtime-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-stdio-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-string-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-time-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-utility-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-eventing-provider-l1-1-0.dll
|   |   |   |   |   |       
|   |   |   |   |   +---u..salcrt-apifwd-vista_6.0.6002.23798
|   |   |   |   |   |       api-ms-win-core-console-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-datetime-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-debug-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-errorhandling-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-file-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-file-l1-2-0.dll
|   |   |   |   |   |       api-ms-win-core-file-l2-1-0.dll
|   |   |   |   |   |       api-ms-win-core-handle-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-heap-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-interlocked-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-libraryloader-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-localization-l1-2-0.dll
|   |   |   |   |   |       api-ms-win-core-memory-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-namedpipe-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-profile-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-rtlsupport-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-string-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-synch-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-synch-l1-2-0.dll
|   |   |   |   |   |       api-ms-win-core-sysinfo-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-timezone-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-util-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-xstate-l2-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-conio-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-convert-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-environment-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-heap-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-locale-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-math-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-private-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-process-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-runtime-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-stdio-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-string-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-time-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-utility-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-eventing-provider-l1-1-0.dll
|   |   |   |   |   |       
|   |   |   |   |   +---ucrt_6.0.6002.19488
|   |   |   |   |   |       ucrtbase.dll
|   |   |   |   |   |       
|   |   |   |   |   \---ucrt_6.0.6002.23798
|   |   |   |   |           ucrtbase.dll
|   |   |   |   |           
|   |   |   |   \---x86
|   |   |   |       +---u..salcrt-apifwd-vista_6.0.6002.19488
|   |   |   |       |       api-ms-win-core-console-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-datetime-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-debug-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-errorhandling-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-file-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-file-l1-2-0.dll
|   |   |   |       |       api-ms-win-core-file-l2-1-0.dll
|   |   |   |       |       api-ms-win-core-handle-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-heap-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-interlocked-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-libraryloader-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-localization-l1-2-0.dll
|   |   |   |       |       api-ms-win-core-memory-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-namedpipe-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-profile-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-rtlsupport-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-string-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-synch-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-synch-l1-2-0.dll
|   |   |   |       |       api-ms-win-core-sysinfo-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-timezone-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-util-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-xstate-l2-1-0.dll
|   |   |   |       |       api-ms-win-crt-conio-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-convert-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-environment-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-heap-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-locale-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-math-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-private-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-process-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-runtime-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-stdio-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-string-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-time-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-utility-l1-1-0.dll
|   |   |   |       |       api-ms-win-eventing-provider-l1-1-0.dll
|   |   |   |       |       
|   |   |   |       +---u..salcrt-apifwd-vista_6.0.6002.23798
|   |   |   |       |       api-ms-win-core-console-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-datetime-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-debug-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-errorhandling-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-file-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-file-l1-2-0.dll
|   |   |   |       |       api-ms-win-core-file-l2-1-0.dll
|   |   |   |       |       api-ms-win-core-handle-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-heap-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-interlocked-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-libraryloader-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-localization-l1-2-0.dll
|   |   |   |       |       api-ms-win-core-memory-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-namedpipe-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-profile-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-rtlsupport-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-string-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-synch-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-synch-l1-2-0.dll
|   |   |   |       |       api-ms-win-core-sysinfo-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-timezone-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-util-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-xstate-l2-1-0.dll
|   |   |   |       |       api-ms-win-crt-conio-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-convert-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-environment-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-heap-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-locale-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-math-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-private-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-process-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-runtime-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-stdio-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-string-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-time-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-utility-l1-1-0.dll
|   |   |   |       |       api-ms-win-eventing-provider-l1-1-0.dll
|   |   |   |       |       
|   |   |   |       +---ucrt_6.0.6002.19488
|   |   |   |       |       ucrtbase.dll
|   |   |   |       |       
|   |   |   |       \---ucrt_6.0.6002.23798
|   |   |   |               ucrtbase.dll
|   |   |   |               
|   |   |   +---_Windows6.1-KB2999226-x64.msu_
|   |   |   |   +---JUNK
|   |   |   |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.1.1.7.cat
|   |   |   |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.1.1.7.mum
|   |   |   |   |       package_1_for_kb2999226~31bf3856ad364e35~amd64~~6.1.1.7.cat
|   |   |   |   |       package_1_for_kb2999226~31bf3856ad364e35~amd64~~6.1.1.7.mum
|   |   |   |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.1.1.7.cat
|   |   |   |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.1.1.7.mum
|   |   |   |   |       package_2_for_kb2999226~31bf3856ad364e35~amd64~~6.1.1.7.cat
|   |   |   |   |       package_2_for_kb2999226~31bf3856ad364e35~amd64~~6.1.1.7.mum
|   |   |   |   |       package_for_kb2999226_sp1_bf~31bf3856ad364e35~amd64~~6.1.1.7.cat
|   |   |   |   |       package_for_kb2999226_sp1_bf~31bf3856ad364e35~amd64~~6.1.1.7.mum
|   |   |   |   |       package_for_kb2999226_sp1~31bf3856ad364e35~amd64~~6.1.1.7.cat
|   |   |   |   |       package_for_kb2999226_sp1~31bf3856ad364e35~amd64~~6.1.1.7.mum
|   |   |   |   |       update-bf.cat
|   |   |   |   |       update-bf.mum
|   |   |   |   |       update.cat
|   |   |   |   |       update.mum
|   |   |   |   |       
|   |   |   |   +---MSIL
|   |   |   |   +---PATCH
|   |   |   |   |       Windows6.1-KB2999226-x64-pkgProperties.txt
|   |   |   |   |       Windows6.1-KB2999226-x64.cab
|   |   |   |   |       Windows6.1-KB2999226-x64.xml
|   |   |   |   |       WSUSSCAN.cab
|   |   |   |   |       
|   |   |   |   +---WOW64
|   |   |   |   +---x64
|   |   |   |   |   +---u..rsalcrt-apifwd-win7_6.1.7601.18972
|   |   |   |   |   |       api-ms-win-core-file-l1-2-0.dll
|   |   |   |   |   |       api-ms-win-core-file-l2-1-0.dll
|   |   |   |   |   |       api-ms-win-core-localization-l1-2-0.dll
|   |   |   |   |   |       api-ms-win-core-synch-l1-2-0.dll
|   |   |   |   |   |       api-ms-win-core-timezone-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-xstate-l2-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-conio-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-convert-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-environment-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-heap-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-locale-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-math-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-private-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-process-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-runtime-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-stdio-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-string-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-time-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-utility-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-eventing-provider-l1-1-0.dll
|   |   |   |   |   |       
|   |   |   |   |   +---u..rsalcrt-apifwd-win7_6.1.7601.23175
|   |   |   |   |   |       api-ms-win-core-file-l1-2-0.dll
|   |   |   |   |   |       api-ms-win-core-file-l2-1-0.dll
|   |   |   |   |   |       api-ms-win-core-localization-l1-2-0.dll
|   |   |   |   |   |       api-ms-win-core-synch-l1-2-0.dll
|   |   |   |   |   |       api-ms-win-core-timezone-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-core-xstate-l2-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-conio-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-convert-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-environment-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-heap-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-locale-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-math-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-private-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-process-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-runtime-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-stdio-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-string-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-time-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-utility-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-eventing-provider-l1-1-0.dll
|   |   |   |   |   |       
|   |   |   |   |   +---ucrt_6.1.7601.18972
|   |   |   |   |   |       ucrtbase.dll
|   |   |   |   |   |       
|   |   |   |   |   \---ucrt_6.1.7601.23175
|   |   |   |   |           ucrtbase.dll
|   |   |   |   |           
|   |   |   |   \---x86
|   |   |   |       +---u..rsalcrt-apifwd-win7_6.1.7601.18972
|   |   |   |       |       api-ms-win-core-file-l1-2-0.dll
|   |   |   |       |       api-ms-win-core-file-l2-1-0.dll
|   |   |   |       |       api-ms-win-core-localization-l1-2-0.dll
|   |   |   |       |       api-ms-win-core-synch-l1-2-0.dll
|   |   |   |       |       api-ms-win-core-timezone-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-xstate-l2-1-0.dll
|   |   |   |       |       api-ms-win-crt-conio-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-convert-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-environment-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-heap-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-locale-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-math-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-private-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-process-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-runtime-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-stdio-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-string-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-time-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-utility-l1-1-0.dll
|   |   |   |       |       api-ms-win-eventing-provider-l1-1-0.dll
|   |   |   |       |       
|   |   |   |       +---u..rsalcrt-apifwd-win7_6.1.7601.23175
|   |   |   |       |       api-ms-win-core-file-l1-2-0.dll
|   |   |   |       |       api-ms-win-core-file-l2-1-0.dll
|   |   |   |       |       api-ms-win-core-localization-l1-2-0.dll
|   |   |   |       |       api-ms-win-core-synch-l1-2-0.dll
|   |   |   |       |       api-ms-win-core-timezone-l1-1-0.dll
|   |   |   |       |       api-ms-win-core-xstate-l2-1-0.dll
|   |   |   |       |       api-ms-win-crt-conio-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-convert-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-environment-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-heap-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-locale-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-math-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-private-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-process-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-runtime-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-stdio-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-string-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-time-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-utility-l1-1-0.dll
|   |   |   |       |       api-ms-win-eventing-provider-l1-1-0.dll
|   |   |   |       |       
|   |   |   |       +---ucrt_6.1.7601.18972
|   |   |   |       |       ucrtbase.dll
|   |   |   |       |       
|   |   |   |       \---ucrt_6.1.7601.23175
|   |   |   |               ucrtbase.dll
|   |   |   |               
|   |   |   +---_Windows8-RT-KB2999226-x64.msu_
|   |   |   |   +---JUNK
|   |   |   |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.2.1.9.cat
|   |   |   |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.2.1.9.mum
|   |   |   |   |       package_1_for_kb2999226~31bf3856ad364e35~amd64~~6.2.1.9.cat
|   |   |   |   |       package_1_for_kb2999226~31bf3856ad364e35~amd64~~6.2.1.9.mum
|   |   |   |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.2.1.9.cat
|   |   |   |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.2.1.9.mum
|   |   |   |   |       package_2_for_kb2999226~31bf3856ad364e35~amd64~~6.2.1.9.cat
|   |   |   |   |       package_2_for_kb2999226~31bf3856ad364e35~amd64~~6.2.1.9.mum
|   |   |   |   |       package_for_kb2999226_rtm_bf~31bf3856ad364e35~amd64~~6.2.1.9.cat
|   |   |   |   |       package_for_kb2999226_rtm_bf~31bf3856ad364e35~amd64~~6.2.1.9.mum
|   |   |   |   |       package_for_kb2999226_rtm~31bf3856ad364e35~amd64~~6.2.1.9.cat
|   |   |   |   |       package_for_kb2999226_rtm~31bf3856ad364e35~amd64~~6.2.1.9.mum
|   |   |   |   |       update-bf.cat
|   |   |   |   |       update-bf.mum
|   |   |   |   |       update.cat
|   |   |   |   |       update.mum
|   |   |   |   |       
|   |   |   |   +---MSIL
|   |   |   |   +---PATCH
|   |   |   |   |       Windows8-RT-KB2999226-x64-pkgProperties.txt
|   |   |   |   |       Windows8-RT-KB2999226-x64.cab
|   |   |   |   |       Windows8-RT-KB2999226-x64.xml
|   |   |   |   |       WSUSSCAN.cab
|   |   |   |   |       
|   |   |   |   +---WOW64
|   |   |   |   +---x64
|   |   |   |   |   +---u..rsalcrt-apifwd-win8_6.2.9200.17488
|   |   |   |   |   |       api-ms-win-core-xstate-l2-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-conio-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-convert-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-environment-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-heap-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-locale-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-math-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-private-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-process-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-runtime-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-stdio-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-string-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-time-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-utility-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-eventing-provider-l1-1-0.dll
|   |   |   |   |   |       
|   |   |   |   |   +---u..rsalcrt-apifwd-win8_6.2.9200.21602
|   |   |   |   |   |       api-ms-win-core-xstate-l2-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-conio-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-convert-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-environment-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-heap-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-locale-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-math-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-private-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-process-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-runtime-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-stdio-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-string-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-time-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-crt-utility-l1-1-0.dll
|   |   |   |   |   |       api-ms-win-eventing-provider-l1-1-0.dll
|   |   |   |   |   |       
|   |   |   |   |   +---ucrt_6.2.9200.17488
|   |   |   |   |   |       ucrtbase.dll
|   |   |   |   |   |       
|   |   |   |   |   \---ucrt_6.2.9200.21602
|   |   |   |   |           ucrtbase.dll
|   |   |   |   |           
|   |   |   |   \---x86
|   |   |   |       +---u..rsalcrt-apifwd-win8_6.2.9200.17488
|   |   |   |       |       api-ms-win-core-xstate-l2-1-0.dll
|   |   |   |       |       api-ms-win-crt-conio-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-convert-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-environment-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-heap-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-locale-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-math-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-private-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-process-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-runtime-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-stdio-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-string-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-time-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-utility-l1-1-0.dll
|   |   |   |       |       api-ms-win-eventing-provider-l1-1-0.dll
|   |   |   |       |       
|   |   |   |       +---u..rsalcrt-apifwd-win8_6.2.9200.21602
|   |   |   |       |       api-ms-win-core-xstate-l2-1-0.dll
|   |   |   |       |       api-ms-win-crt-conio-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-convert-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-environment-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-heap-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-locale-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-math-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-private-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-process-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-runtime-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-stdio-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-string-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-time-l1-1-0.dll
|   |   |   |       |       api-ms-win-crt-utility-l1-1-0.dll
|   |   |   |       |       api-ms-win-eventing-provider-l1-1-0.dll
|   |   |   |       |       
|   |   |   |       +---ucrt_6.2.9200.17488
|   |   |   |       |       ucrtbase.dll
|   |   |   |       |       
|   |   |   |       \---ucrt_6.2.9200.21602
|   |   |   |               ucrtbase.dll
|   |   |   |               
|   |   |   \---_Windows8.1-KB2999226-x64.msu_
|   |   |       +---JUNK
|   |   |       |       package_1_for_kb2999226~31bf3856ad364e35~amd64~~6.3.1.9.cat
|   |   |       |       package_1_for_kb2999226~31bf3856ad364e35~amd64~~6.3.1.9.mum
|   |   |       |       package_for_kb2999226_rtm_gm~31bf3856ad364e35~amd64~~6.3.1.9.cat
|   |   |       |       package_for_kb2999226_rtm_gm~31bf3856ad364e35~amd64~~6.3.1.9.mum
|   |   |       |       package_for_kb2999226_rtm~31bf3856ad364e35~amd64~~6.3.1.9.cat
|   |   |       |       package_for_kb2999226_rtm~31bf3856ad364e35~amd64~~6.3.1.9.mum
|   |   |       |       update.cat
|   |   |       |       update.mum
|   |   |       |       
|   |   |       +---MSIL
|   |   |       +---PATCH
|   |   |       |       Windows8.1-KB2999226-x64-pkgProperties.txt
|   |   |       |       Windows8.1-KB2999226-x64.cab
|   |   |       |       Windows8.1-KB2999226-x64.xml
|   |   |       |       WSUSSCAN.cab
|   |   |       |       
|   |   |       +---WOW64
|   |   |       +---x64
|   |   |       |   +---u..lcrt-apifwd-winblue_6.3.9600.18036
|   |   |       |   |       api-ms-win-crt-conio-l1-1-0.dll
|   |   |       |   |       api-ms-win-crt-convert-l1-1-0.dll
|   |   |       |   |       api-ms-win-crt-environment-l1-1-0.dll
|   |   |       |   |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |   |       |   |       api-ms-win-crt-heap-l1-1-0.dll
|   |   |       |   |       api-ms-win-crt-locale-l1-1-0.dll
|   |   |       |   |       api-ms-win-crt-math-l1-1-0.dll
|   |   |       |   |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |   |       |   |       api-ms-win-crt-private-l1-1-0.dll
|   |   |       |   |       api-ms-win-crt-process-l1-1-0.dll
|   |   |       |   |       api-ms-win-crt-runtime-l1-1-0.dll
|   |   |       |   |       api-ms-win-crt-stdio-l1-1-0.dll
|   |   |       |   |       api-ms-win-crt-string-l1-1-0.dll
|   |   |       |   |       api-ms-win-crt-time-l1-1-0.dll
|   |   |       |   |       api-ms-win-crt-utility-l1-1-0.dll
|   |   |       |   |       
|   |   |       |   \---ucrt_6.3.9600.18036
|   |   |       |           ucrtbase.dll
|   |   |       |           
|   |   |       \---x86
|   |   |           +---u..lcrt-apifwd-winblue_6.3.9600.18036
|   |   |           |       api-ms-win-crt-conio-l1-1-0.dll
|   |   |           |       api-ms-win-crt-convert-l1-1-0.dll
|   |   |           |       api-ms-win-crt-environment-l1-1-0.dll
|   |   |           |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |   |           |       api-ms-win-crt-heap-l1-1-0.dll
|   |   |           |       api-ms-win-crt-locale-l1-1-0.dll
|   |   |           |       api-ms-win-crt-math-l1-1-0.dll
|   |   |           |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |   |           |       api-ms-win-crt-private-l1-1-0.dll
|   |   |           |       api-ms-win-crt-process-l1-1-0.dll
|   |   |           |       api-ms-win-crt-runtime-l1-1-0.dll
|   |   |           |       api-ms-win-crt-stdio-l1-1-0.dll
|   |   |           |       api-ms-win-crt-string-l1-1-0.dll
|   |   |           |       api-ms-win-crt-time-l1-1-0.dll
|   |   |           |       api-ms-win-crt-utility-l1-1-0.dll
|   |   |           |       
|   |   |           \---ucrt_6.3.9600.18036
|   |   |                   ucrtbase.dll
|   |   |                   
|   |   \---x86
|   |       +---_Windows6.0-KB2999226-x86.msu_
|   |       |   +---JUNK
|   |       |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_1_for_kb2999226~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_1_for_kb2999226~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_2_for_kb2999226~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_2_for_kb2999226~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_3_for_kb2999226_bf~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_3_for_kb2999226_bf~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_3_for_kb2999226~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_3_for_kb2999226~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_for_kb2999226_client_2_bf~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_for_kb2999226_client_2_bf~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_for_kb2999226_client_2~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_for_kb2999226_client_2~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_for_kb2999226_client_bf~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_for_kb2999226_client_bf~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_for_kb2999226_client~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_for_kb2999226_client~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_for_kb2999226_sc_1_bf~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_for_kb2999226_sc_1_bf~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_for_kb2999226_sc_1~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_for_kb2999226_sc_1~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_for_kb2999226_sc_bf~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_for_kb2999226_sc_bf~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_for_kb2999226_sc~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_for_kb2999226_sc~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_for_kb2999226_server_1_bf~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_for_kb2999226_server_1_bf~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_for_kb2999226_server_1~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_for_kb2999226_server_1~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_for_kb2999226_server_bf~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_for_kb2999226_server_bf~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       package_for_kb2999226_server~31bf3856ad364e35~x86~~6.0.1.6.cat
|   |       |   |       package_for_kb2999226_server~31bf3856ad364e35~x86~~6.0.1.6.mum
|   |       |   |       update-bf.cat
|   |       |   |       update-bf.mum
|   |       |   |       update.cat
|   |       |   |       update.mum
|   |       |   |       
|   |       |   +---MSIL
|   |       |   +---PATCH
|   |       |   |       Windows6.0-KB2999226-x86-pkgProperties.txt
|   |       |   |       Windows6.0-KB2999226-x86.cab
|   |       |   |       Windows6.0-KB2999226-x86.xml
|   |       |   |       WSUSSCAN.cab
|   |       |   |       
|   |       |   +---WOW64
|   |       |   +---x64
|   |       |   \---x86
|   |       |       +---u..salcrt-apifwd-vista_6.0.6002.19488
|   |       |       |       api-ms-win-core-console-l1-1-0.dll
|   |       |       |       api-ms-win-core-datetime-l1-1-0.dll
|   |       |       |       api-ms-win-core-debug-l1-1-0.dll
|   |       |       |       api-ms-win-core-errorhandling-l1-1-0.dll
|   |       |       |       api-ms-win-core-file-l1-1-0.dll
|   |       |       |       api-ms-win-core-file-l1-2-0.dll
|   |       |       |       api-ms-win-core-file-l2-1-0.dll
|   |       |       |       api-ms-win-core-handle-l1-1-0.dll
|   |       |       |       api-ms-win-core-heap-l1-1-0.dll
|   |       |       |       api-ms-win-core-interlocked-l1-1-0.dll
|   |       |       |       api-ms-win-core-libraryloader-l1-1-0.dll
|   |       |       |       api-ms-win-core-localization-l1-2-0.dll
|   |       |       |       api-ms-win-core-memory-l1-1-0.dll
|   |       |       |       api-ms-win-core-namedpipe-l1-1-0.dll
|   |       |       |       api-ms-win-core-profile-l1-1-0.dll
|   |       |       |       api-ms-win-core-rtlsupport-l1-1-0.dll
|   |       |       |       api-ms-win-core-string-l1-1-0.dll
|   |       |       |       api-ms-win-core-synch-l1-1-0.dll
|   |       |       |       api-ms-win-core-synch-l1-2-0.dll
|   |       |       |       api-ms-win-core-sysinfo-l1-1-0.dll
|   |       |       |       api-ms-win-core-timezone-l1-1-0.dll
|   |       |       |       api-ms-win-core-util-l1-1-0.dll
|   |       |       |       api-ms-win-core-xstate-l2-1-0.dll
|   |       |       |       api-ms-win-crt-conio-l1-1-0.dll
|   |       |       |       api-ms-win-crt-convert-l1-1-0.dll
|   |       |       |       api-ms-win-crt-environment-l1-1-0.dll
|   |       |       |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |       |       |       api-ms-win-crt-heap-l1-1-0.dll
|   |       |       |       api-ms-win-crt-locale-l1-1-0.dll
|   |       |       |       api-ms-win-crt-math-l1-1-0.dll
|   |       |       |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |       |       |       api-ms-win-crt-private-l1-1-0.dll
|   |       |       |       api-ms-win-crt-process-l1-1-0.dll
|   |       |       |       api-ms-win-crt-runtime-l1-1-0.dll
|   |       |       |       api-ms-win-crt-stdio-l1-1-0.dll
|   |       |       |       api-ms-win-crt-string-l1-1-0.dll
|   |       |       |       api-ms-win-crt-time-l1-1-0.dll
|   |       |       |       api-ms-win-crt-utility-l1-1-0.dll
|   |       |       |       api-ms-win-eventing-provider-l1-1-0.dll
|   |       |       |       
|   |       |       +---u..salcrt-apifwd-vista_6.0.6002.23798
|   |       |       |       api-ms-win-core-console-l1-1-0.dll
|   |       |       |       api-ms-win-core-datetime-l1-1-0.dll
|   |       |       |       api-ms-win-core-debug-l1-1-0.dll
|   |       |       |       api-ms-win-core-errorhandling-l1-1-0.dll
|   |       |       |       api-ms-win-core-file-l1-1-0.dll
|   |       |       |       api-ms-win-core-file-l1-2-0.dll
|   |       |       |       api-ms-win-core-file-l2-1-0.dll
|   |       |       |       api-ms-win-core-handle-l1-1-0.dll
|   |       |       |       api-ms-win-core-heap-l1-1-0.dll
|   |       |       |       api-ms-win-core-interlocked-l1-1-0.dll
|   |       |       |       api-ms-win-core-libraryloader-l1-1-0.dll
|   |       |       |       api-ms-win-core-localization-l1-2-0.dll
|   |       |       |       api-ms-win-core-memory-l1-1-0.dll
|   |       |       |       api-ms-win-core-namedpipe-l1-1-0.dll
|   |       |       |       api-ms-win-core-profile-l1-1-0.dll
|   |       |       |       api-ms-win-core-rtlsupport-l1-1-0.dll
|   |       |       |       api-ms-win-core-string-l1-1-0.dll
|   |       |       |       api-ms-win-core-synch-l1-1-0.dll
|   |       |       |       api-ms-win-core-synch-l1-2-0.dll
|   |       |       |       api-ms-win-core-sysinfo-l1-1-0.dll
|   |       |       |       api-ms-win-core-timezone-l1-1-0.dll
|   |       |       |       api-ms-win-core-util-l1-1-0.dll
|   |       |       |       api-ms-win-core-xstate-l2-1-0.dll
|   |       |       |       api-ms-win-crt-conio-l1-1-0.dll
|   |       |       |       api-ms-win-crt-convert-l1-1-0.dll
|   |       |       |       api-ms-win-crt-environment-l1-1-0.dll
|   |       |       |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |       |       |       api-ms-win-crt-heap-l1-1-0.dll
|   |       |       |       api-ms-win-crt-locale-l1-1-0.dll
|   |       |       |       api-ms-win-crt-math-l1-1-0.dll
|   |       |       |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |       |       |       api-ms-win-crt-private-l1-1-0.dll
|   |       |       |       api-ms-win-crt-process-l1-1-0.dll
|   |       |       |       api-ms-win-crt-runtime-l1-1-0.dll
|   |       |       |       api-ms-win-crt-stdio-l1-1-0.dll
|   |       |       |       api-ms-win-crt-string-l1-1-0.dll
|   |       |       |       api-ms-win-crt-time-l1-1-0.dll
|   |       |       |       api-ms-win-crt-utility-l1-1-0.dll
|   |       |       |       api-ms-win-eventing-provider-l1-1-0.dll
|   |       |       |       
|   |       |       +---ucrt_6.0.6002.19488
|   |       |       |       ucrtbase.dll
|   |       |       |       
|   |       |       \---ucrt_6.0.6002.23798
|   |       |               ucrtbase.dll
|   |       |               
|   |       +---_Windows6.1-KB2999226-x86.msu_
|   |       |   +---JUNK
|   |       |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~x86~~6.1.1.7.cat
|   |       |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~x86~~6.1.1.7.mum
|   |       |   |       package_1_for_kb2999226~31bf3856ad364e35~x86~~6.1.1.7.cat
|   |       |   |       package_1_for_kb2999226~31bf3856ad364e35~x86~~6.1.1.7.mum
|   |       |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~x86~~6.1.1.7.cat
|   |       |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~x86~~6.1.1.7.mum
|   |       |   |       package_2_for_kb2999226~31bf3856ad364e35~x86~~6.1.1.7.cat
|   |       |   |       package_2_for_kb2999226~31bf3856ad364e35~x86~~6.1.1.7.mum
|   |       |   |       package_for_kb2999226_sp1_bf~31bf3856ad364e35~x86~~6.1.1.7.cat
|   |       |   |       package_for_kb2999226_sp1_bf~31bf3856ad364e35~x86~~6.1.1.7.mum
|   |       |   |       package_for_kb2999226_sp1~31bf3856ad364e35~x86~~6.1.1.7.cat
|   |       |   |       package_for_kb2999226_sp1~31bf3856ad364e35~x86~~6.1.1.7.mum
|   |       |   |       update-bf.cat
|   |       |   |       update-bf.mum
|   |       |   |       update.cat
|   |       |   |       update.mum
|   |       |   |       
|   |       |   +---MSIL
|   |       |   +---PATCH
|   |       |   |       Windows6.1-KB2999226-x86-pkgProperties.txt
|   |       |   |       Windows6.1-KB2999226-x86.cab
|   |       |   |       Windows6.1-KB2999226-x86.xml
|   |       |   |       WSUSSCAN.cab
|   |       |   |       
|   |       |   +---WOW64
|   |       |   +---x64
|   |       |   \---x86
|   |       |       +---u..rsalcrt-apifwd-win7_6.1.7601.18972
|   |       |       |       api-ms-win-core-file-l1-2-0.dll
|   |       |       |       api-ms-win-core-file-l2-1-0.dll
|   |       |       |       api-ms-win-core-localization-l1-2-0.dll
|   |       |       |       api-ms-win-core-synch-l1-2-0.dll
|   |       |       |       api-ms-win-core-timezone-l1-1-0.dll
|   |       |       |       api-ms-win-core-xstate-l2-1-0.dll
|   |       |       |       api-ms-win-crt-conio-l1-1-0.dll
|   |       |       |       api-ms-win-crt-convert-l1-1-0.dll
|   |       |       |       api-ms-win-crt-environment-l1-1-0.dll
|   |       |       |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |       |       |       api-ms-win-crt-heap-l1-1-0.dll
|   |       |       |       api-ms-win-crt-locale-l1-1-0.dll
|   |       |       |       api-ms-win-crt-math-l1-1-0.dll
|   |       |       |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |       |       |       api-ms-win-crt-private-l1-1-0.dll
|   |       |       |       api-ms-win-crt-process-l1-1-0.dll
|   |       |       |       api-ms-win-crt-runtime-l1-1-0.dll
|   |       |       |       api-ms-win-crt-stdio-l1-1-0.dll
|   |       |       |       api-ms-win-crt-string-l1-1-0.dll
|   |       |       |       api-ms-win-crt-time-l1-1-0.dll
|   |       |       |       api-ms-win-crt-utility-l1-1-0.dll
|   |       |       |       api-ms-win-eventing-provider-l1-1-0.dll
|   |       |       |       
|   |       |       +---u..rsalcrt-apifwd-win7_6.1.7601.23175
|   |       |       |       api-ms-win-core-file-l1-2-0.dll
|   |       |       |       api-ms-win-core-file-l2-1-0.dll
|   |       |       |       api-ms-win-core-localization-l1-2-0.dll
|   |       |       |       api-ms-win-core-synch-l1-2-0.dll
|   |       |       |       api-ms-win-core-timezone-l1-1-0.dll
|   |       |       |       api-ms-win-core-xstate-l2-1-0.dll
|   |       |       |       api-ms-win-crt-conio-l1-1-0.dll
|   |       |       |       api-ms-win-crt-convert-l1-1-0.dll
|   |       |       |       api-ms-win-crt-environment-l1-1-0.dll
|   |       |       |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |       |       |       api-ms-win-crt-heap-l1-1-0.dll
|   |       |       |       api-ms-win-crt-locale-l1-1-0.dll
|   |       |       |       api-ms-win-crt-math-l1-1-0.dll
|   |       |       |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |       |       |       api-ms-win-crt-private-l1-1-0.dll
|   |       |       |       api-ms-win-crt-process-l1-1-0.dll
|   |       |       |       api-ms-win-crt-runtime-l1-1-0.dll
|   |       |       |       api-ms-win-crt-stdio-l1-1-0.dll
|   |       |       |       api-ms-win-crt-string-l1-1-0.dll
|   |       |       |       api-ms-win-crt-time-l1-1-0.dll
|   |       |       |       api-ms-win-crt-utility-l1-1-0.dll
|   |       |       |       api-ms-win-eventing-provider-l1-1-0.dll
|   |       |       |       
|   |       |       +---ucrt_6.1.7601.18972
|   |       |       |       ucrtbase.dll
|   |       |       |       
|   |       |       \---ucrt_6.1.7601.23175
|   |       |               ucrtbase.dll
|   |       |               
|   |       +---_Windows8-RT-KB2999226-x86.msu_
|   |       |   +---JUNK
|   |       |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~x86~~6.2.1.9.cat
|   |       |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~x86~~6.2.1.9.mum
|   |       |   |       package_1_for_kb2999226~31bf3856ad364e35~x86~~6.2.1.9.cat
|   |       |   |       package_1_for_kb2999226~31bf3856ad364e35~x86~~6.2.1.9.mum
|   |       |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~x86~~6.2.1.9.cat
|   |       |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~x86~~6.2.1.9.mum
|   |       |   |       package_2_for_kb2999226~31bf3856ad364e35~x86~~6.2.1.9.cat
|   |       |   |       package_2_for_kb2999226~31bf3856ad364e35~x86~~6.2.1.9.mum
|   |       |   |       package_for_kb2999226_rtm_bf~31bf3856ad364e35~x86~~6.2.1.9.cat
|   |       |   |       package_for_kb2999226_rtm_bf~31bf3856ad364e35~x86~~6.2.1.9.mum
|   |       |   |       package_for_kb2999226_rtm~31bf3856ad364e35~x86~~6.2.1.9.cat
|   |       |   |       package_for_kb2999226_rtm~31bf3856ad364e35~x86~~6.2.1.9.mum
|   |       |   |       update-bf.cat
|   |       |   |       update-bf.mum
|   |       |   |       update.cat
|   |       |   |       update.mum
|   |       |   |       
|   |       |   +---MSIL
|   |       |   +---PATCH
|   |       |   |       Windows8-RT-KB2999226-x86-pkgProperties.txt
|   |       |   |       Windows8-RT-KB2999226-x86.cab
|   |       |   |       Windows8-RT-KB2999226-x86.xml
|   |       |   |       WSUSSCAN.cab
|   |       |   |       
|   |       |   +---WOW64
|   |       |   +---x64
|   |       |   \---x86
|   |       |       +---u..rsalcrt-apifwd-win8_6.2.9200.17488
|   |       |       |       api-ms-win-core-xstate-l2-1-0.dll
|   |       |       |       api-ms-win-crt-conio-l1-1-0.dll
|   |       |       |       api-ms-win-crt-convert-l1-1-0.dll
|   |       |       |       api-ms-win-crt-environment-l1-1-0.dll
|   |       |       |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |       |       |       api-ms-win-crt-heap-l1-1-0.dll
|   |       |       |       api-ms-win-crt-locale-l1-1-0.dll
|   |       |       |       api-ms-win-crt-math-l1-1-0.dll
|   |       |       |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |       |       |       api-ms-win-crt-private-l1-1-0.dll
|   |       |       |       api-ms-win-crt-process-l1-1-0.dll
|   |       |       |       api-ms-win-crt-runtime-l1-1-0.dll
|   |       |       |       api-ms-win-crt-stdio-l1-1-0.dll
|   |       |       |       api-ms-win-crt-string-l1-1-0.dll
|   |       |       |       api-ms-win-crt-time-l1-1-0.dll
|   |       |       |       api-ms-win-crt-utility-l1-1-0.dll
|   |       |       |       api-ms-win-eventing-provider-l1-1-0.dll
|   |       |       |       
|   |       |       +---u..rsalcrt-apifwd-win8_6.2.9200.21602
|   |       |       |       api-ms-win-core-xstate-l2-1-0.dll
|   |       |       |       api-ms-win-crt-conio-l1-1-0.dll
|   |       |       |       api-ms-win-crt-convert-l1-1-0.dll
|   |       |       |       api-ms-win-crt-environment-l1-1-0.dll
|   |       |       |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |       |       |       api-ms-win-crt-heap-l1-1-0.dll
|   |       |       |       api-ms-win-crt-locale-l1-1-0.dll
|   |       |       |       api-ms-win-crt-math-l1-1-0.dll
|   |       |       |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |       |       |       api-ms-win-crt-private-l1-1-0.dll
|   |       |       |       api-ms-win-crt-process-l1-1-0.dll
|   |       |       |       api-ms-win-crt-runtime-l1-1-0.dll
|   |       |       |       api-ms-win-crt-stdio-l1-1-0.dll
|   |       |       |       api-ms-win-crt-string-l1-1-0.dll
|   |       |       |       api-ms-win-crt-time-l1-1-0.dll
|   |       |       |       api-ms-win-crt-utility-l1-1-0.dll
|   |       |       |       api-ms-win-eventing-provider-l1-1-0.dll
|   |       |       |       
|   |       |       +---ucrt_6.2.9200.17488
|   |       |       |       ucrtbase.dll
|   |       |       |       
|   |       |       \---ucrt_6.2.9200.21602
|   |       |               ucrtbase.dll
|   |       |               
|   |       \---_Windows8.1-KB2999226-x86.msu_
|   |           +---JUNK
|   |           |       package_1_for_kb2999226~31bf3856ad364e35~x86~~6.3.1.9.cat
|   |           |       package_1_for_kb2999226~31bf3856ad364e35~x86~~6.3.1.9.mum
|   |           |       package_for_kb2999226_rtm_gm~31bf3856ad364e35~x86~~6.3.1.9.cat
|   |           |       package_for_kb2999226_rtm_gm~31bf3856ad364e35~x86~~6.3.1.9.mum
|   |           |       package_for_kb2999226_rtm~31bf3856ad364e35~x86~~6.3.1.9.cat
|   |           |       package_for_kb2999226_rtm~31bf3856ad364e35~x86~~6.3.1.9.mum
|   |           |       update.cat
|   |           |       update.mum
|   |           |       
|   |           +---MSIL
|   |           +---PATCH
|   |           |       Windows8.1-KB2999226-x86-pkgProperties.txt
|   |           |       Windows8.1-KB2999226-x86.cab
|   |           |       Windows8.1-KB2999226-x86.xml
|   |           |       WSUSSCAN.cab
|   |           |       
|   |           +---WOW64
|   |           +---x64
|   |           \---x86
|   |               +---u..lcrt-apifwd-winblue_6.3.9600.18036
|   |               |       api-ms-win-crt-conio-l1-1-0.dll
|   |               |       api-ms-win-crt-convert-l1-1-0.dll
|   |               |       api-ms-win-crt-environment-l1-1-0.dll
|   |               |       api-ms-win-crt-filesystem-l1-1-0.dll
|   |               |       api-ms-win-crt-heap-l1-1-0.dll
|   |               |       api-ms-win-crt-locale-l1-1-0.dll
|   |               |       api-ms-win-crt-math-l1-1-0.dll
|   |               |       api-ms-win-crt-multibyte-l1-1-0.dll
|   |               |       api-ms-win-crt-private-l1-1-0.dll
|   |               |       api-ms-win-crt-process-l1-1-0.dll
|   |               |       api-ms-win-crt-runtime-l1-1-0.dll
|   |               |       api-ms-win-crt-stdio-l1-1-0.dll
|   |               |       api-ms-win-crt-string-l1-1-0.dll
|   |               |       api-ms-win-crt-time-l1-1-0.dll
|   |               |       api-ms-win-crt-utility-l1-1-0.dll
|   |               |       
|   |               \---ucrt_6.3.9600.18036
|   |                       ucrtbase.dll
|   |                       
|   +---vc_runtimeAdditional_x64
|   |   |   vc_runtimeAdditional_x64.msi
|   |   |   
|   |   \---System64
|   |           mfc140.dll
|   |           mfc140chs.dll
|   |           mfc140cht.dll
|   |           mfc140deu.dll
|   |           mfc140enu.dll
|   |           mfc140esn.dll
|   |           mfc140fra.dll
|   |           mfc140ita.dll
|   |           mfc140jpn.dll
|   |           mfc140kor.dll
|   |           mfc140rus.dll
|   |           mfc140u.dll
|   |           mfcm140.dll
|   |           mfcm140u.dll
|   |           
|   +---vc_runtimeMinimum_x64
|   |   |   vc_runtimeMinimum_x64.msi
|   |   |   
|   |   \---System64
|   |           concrt140.dll
|   |           msvcp140.dll
|   |           msvcp140_1.dll
|   |           msvcp140_2.dll
|   |           msvcp140_atomic_wait.dll
|   |           msvcp140_codecvt_ids.dll
|   |           vcamp140.dll
|   |           vccorlib140.dll
|   |           vcomp140.dll
|   |           vcruntime140.dll
|   |           vcruntime140_1.dll
|   |           
|   \---VC_Runtime_arm64
|       |   VC_Runtime_arm64.msi
|       |   
|       \---System64
|               concrt140.dll
|               mfc140.dll
|               mfc140chs.dll
|               mfc140cht.dll
|               mfc140deu.dll
|               mfc140enu.dll
|               mfc140esn.dll
|               mfc140fra.dll
|               mfc140ita.dll
|               mfc140jpn.dll
|               mfc140kor.dll
|               mfc140rus.dll
|               mfc140u.dll
|               msvcp140.dll
|               msvcp140_1.dll
|               msvcp140_2.dll
|               msvcp140_atomic_wait.dll
|               msvcp140_codecvt_ids.dll
|               vcamp140.dll
|               vccorlib140.dll
|               vcomp140.dll
|               vcruntime140.dll
|               vcruntime140_1.dll
|               
\---Visual Studio 2015, 2017, 2019, and 2022 VC_redist.x86_extracted
    +---Patch
    |   +---x64
    |   |   +---_Windows6.0-KB2999226-x64.msu_
    |   |   |   +---JUNK
    |   |   |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_1_for_kb2999226~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_1_for_kb2999226~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_2_for_kb2999226~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_2_for_kb2999226~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_3_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_3_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_3_for_kb2999226~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_3_for_kb2999226~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_for_kb2999226_client_2_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_for_kb2999226_client_2_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_for_kb2999226_client_2~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_for_kb2999226_client_2~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_for_kb2999226_client_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_for_kb2999226_client_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_for_kb2999226_client~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_for_kb2999226_client~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_for_kb2999226_sc_1_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_for_kb2999226_sc_1_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_for_kb2999226_sc_1~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_for_kb2999226_sc_1~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_for_kb2999226_sc_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_for_kb2999226_sc_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_for_kb2999226_sc~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_for_kb2999226_sc~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_for_kb2999226_server_1_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_for_kb2999226_server_1_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_for_kb2999226_server_1~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_for_kb2999226_server_1~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_for_kb2999226_server_bf~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_for_kb2999226_server_bf~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       package_for_kb2999226_server~31bf3856ad364e35~amd64~~6.0.1.6.cat
    |   |   |   |       package_for_kb2999226_server~31bf3856ad364e35~amd64~~6.0.1.6.mum
    |   |   |   |       update-bf.cat
    |   |   |   |       update-bf.mum
    |   |   |   |       update.cat
    |   |   |   |       update.mum
    |   |   |   |       
    |   |   |   +---MSIL
    |   |   |   +---PATCH
    |   |   |   |       Windows6.0-KB2999226-x64-pkgProperties.txt
    |   |   |   |       Windows6.0-KB2999226-x64.cab
    |   |   |   |       Windows6.0-KB2999226-x64.xml
    |   |   |   |       WSUSSCAN.cab
    |   |   |   |       
    |   |   |   +---WOW64
    |   |   |   +---x64
    |   |   |   |   +---u..salcrt-apifwd-vista_6.0.6002.19488
    |   |   |   |   |       api-ms-win-core-console-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-datetime-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-debug-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-errorhandling-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-file-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-file-l1-2-0.dll
    |   |   |   |   |       api-ms-win-core-file-l2-1-0.dll
    |   |   |   |   |       api-ms-win-core-handle-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-heap-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-interlocked-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-libraryloader-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-localization-l1-2-0.dll
    |   |   |   |   |       api-ms-win-core-memory-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-namedpipe-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-profile-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-rtlsupport-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-string-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-synch-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-synch-l1-2-0.dll
    |   |   |   |   |       api-ms-win-core-sysinfo-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-timezone-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-util-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-xstate-l2-1-0.dll
    |   |   |   |   |       api-ms-win-crt-conio-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-convert-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-environment-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-filesystem-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-heap-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-locale-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-math-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-multibyte-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-private-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-process-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-runtime-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-stdio-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-string-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-time-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-utility-l1-1-0.dll
    |   |   |   |   |       api-ms-win-eventing-provider-l1-1-0.dll
    |   |   |   |   |       
    |   |   |   |   +---u..salcrt-apifwd-vista_6.0.6002.23798
    |   |   |   |   |       api-ms-win-core-console-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-datetime-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-debug-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-errorhandling-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-file-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-file-l1-2-0.dll
    |   |   |   |   |       api-ms-win-core-file-l2-1-0.dll
    |   |   |   |   |       api-ms-win-core-handle-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-heap-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-interlocked-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-libraryloader-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-localization-l1-2-0.dll
    |   |   |   |   |       api-ms-win-core-memory-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-namedpipe-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-profile-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-rtlsupport-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-string-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-synch-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-synch-l1-2-0.dll
    |   |   |   |   |       api-ms-win-core-sysinfo-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-timezone-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-util-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-xstate-l2-1-0.dll
    |   |   |   |   |       api-ms-win-crt-conio-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-convert-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-environment-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-filesystem-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-heap-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-locale-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-math-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-multibyte-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-private-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-process-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-runtime-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-stdio-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-string-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-time-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-utility-l1-1-0.dll
    |   |   |   |   |       api-ms-win-eventing-provider-l1-1-0.dll
    |   |   |   |   |       
    |   |   |   |   +---ucrt_6.0.6002.19488
    |   |   |   |   |       ucrtbase.dll
    |   |   |   |   |       
    |   |   |   |   \---ucrt_6.0.6002.23798
    |   |   |   |           ucrtbase.dll
    |   |   |   |           
    |   |   |   \---x86
    |   |   |       +---u..salcrt-apifwd-vista_6.0.6002.19488
    |   |   |       |       api-ms-win-core-console-l1-1-0.dll
    |   |   |       |       api-ms-win-core-datetime-l1-1-0.dll
    |   |   |       |       api-ms-win-core-debug-l1-1-0.dll
    |   |   |       |       api-ms-win-core-errorhandling-l1-1-0.dll
    |   |   |       |       api-ms-win-core-file-l1-1-0.dll
    |   |   |       |       api-ms-win-core-file-l1-2-0.dll
    |   |   |       |       api-ms-win-core-file-l2-1-0.dll
    |   |   |       |       api-ms-win-core-handle-l1-1-0.dll
    |   |   |       |       api-ms-win-core-heap-l1-1-0.dll
    |   |   |       |       api-ms-win-core-interlocked-l1-1-0.dll
    |   |   |       |       api-ms-win-core-libraryloader-l1-1-0.dll
    |   |   |       |       api-ms-win-core-localization-l1-2-0.dll
    |   |   |       |       api-ms-win-core-memory-l1-1-0.dll
    |   |   |       |       api-ms-win-core-namedpipe-l1-1-0.dll
    |   |   |       |       api-ms-win-core-profile-l1-1-0.dll
    |   |   |       |       api-ms-win-core-rtlsupport-l1-1-0.dll
    |   |   |       |       api-ms-win-core-string-l1-1-0.dll
    |   |   |       |       api-ms-win-core-synch-l1-1-0.dll
    |   |   |       |       api-ms-win-core-synch-l1-2-0.dll
    |   |   |       |       api-ms-win-core-sysinfo-l1-1-0.dll
    |   |   |       |       api-ms-win-core-timezone-l1-1-0.dll
    |   |   |       |       api-ms-win-core-util-l1-1-0.dll
    |   |   |       |       api-ms-win-core-xstate-l2-1-0.dll
    |   |   |       |       api-ms-win-crt-conio-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-convert-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-environment-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-filesystem-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-heap-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-locale-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-math-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-multibyte-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-private-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-process-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-runtime-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-stdio-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-string-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-time-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-utility-l1-1-0.dll
    |   |   |       |       api-ms-win-eventing-provider-l1-1-0.dll
    |   |   |       |       
    |   |   |       +---u..salcrt-apifwd-vista_6.0.6002.23798
    |   |   |       |       api-ms-win-core-console-l1-1-0.dll
    |   |   |       |       api-ms-win-core-datetime-l1-1-0.dll
    |   |   |       |       api-ms-win-core-debug-l1-1-0.dll
    |   |   |       |       api-ms-win-core-errorhandling-l1-1-0.dll
    |   |   |       |       api-ms-win-core-file-l1-1-0.dll
    |   |   |       |       api-ms-win-core-file-l1-2-0.dll
    |   |   |       |       api-ms-win-core-file-l2-1-0.dll
    |   |   |       |       api-ms-win-core-handle-l1-1-0.dll
    |   |   |       |       api-ms-win-core-heap-l1-1-0.dll
    |   |   |       |       api-ms-win-core-interlocked-l1-1-0.dll
    |   |   |       |       api-ms-win-core-libraryloader-l1-1-0.dll
    |   |   |       |       api-ms-win-core-localization-l1-2-0.dll
    |   |   |       |       api-ms-win-core-memory-l1-1-0.dll
    |   |   |       |       api-ms-win-core-namedpipe-l1-1-0.dll
    |   |   |       |       api-ms-win-core-profile-l1-1-0.dll
    |   |   |       |       api-ms-win-core-rtlsupport-l1-1-0.dll
    |   |   |       |       api-ms-win-core-string-l1-1-0.dll
    |   |   |       |       api-ms-win-core-synch-l1-1-0.dll
    |   |   |       |       api-ms-win-core-synch-l1-2-0.dll
    |   |   |       |       api-ms-win-core-sysinfo-l1-1-0.dll
    |   |   |       |       api-ms-win-core-timezone-l1-1-0.dll
    |   |   |       |       api-ms-win-core-util-l1-1-0.dll
    |   |   |       |       api-ms-win-core-xstate-l2-1-0.dll
    |   |   |       |       api-ms-win-crt-conio-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-convert-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-environment-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-filesystem-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-heap-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-locale-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-math-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-multibyte-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-private-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-process-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-runtime-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-stdio-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-string-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-time-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-utility-l1-1-0.dll
    |   |   |       |       api-ms-win-eventing-provider-l1-1-0.dll
    |   |   |       |       
    |   |   |       +---ucrt_6.0.6002.19488
    |   |   |       |       ucrtbase.dll
    |   |   |       |       
    |   |   |       \---ucrt_6.0.6002.23798
    |   |   |               ucrtbase.dll
    |   |   |               
    |   |   +---_Windows6.1-KB2999226-x64.msu_
    |   |   |   +---JUNK
    |   |   |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.1.1.7.cat
    |   |   |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.1.1.7.mum
    |   |   |   |       package_1_for_kb2999226~31bf3856ad364e35~amd64~~6.1.1.7.cat
    |   |   |   |       package_1_for_kb2999226~31bf3856ad364e35~amd64~~6.1.1.7.mum
    |   |   |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.1.1.7.cat
    |   |   |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.1.1.7.mum
    |   |   |   |       package_2_for_kb2999226~31bf3856ad364e35~amd64~~6.1.1.7.cat
    |   |   |   |       package_2_for_kb2999226~31bf3856ad364e35~amd64~~6.1.1.7.mum
    |   |   |   |       package_for_kb2999226_sp1_bf~31bf3856ad364e35~amd64~~6.1.1.7.cat
    |   |   |   |       package_for_kb2999226_sp1_bf~31bf3856ad364e35~amd64~~6.1.1.7.mum
    |   |   |   |       package_for_kb2999226_sp1~31bf3856ad364e35~amd64~~6.1.1.7.cat
    |   |   |   |       package_for_kb2999226_sp1~31bf3856ad364e35~amd64~~6.1.1.7.mum
    |   |   |   |       update-bf.cat
    |   |   |   |       update-bf.mum
    |   |   |   |       update.cat
    |   |   |   |       update.mum
    |   |   |   |       
    |   |   |   +---MSIL
    |   |   |   +---PATCH
    |   |   |   |       Windows6.1-KB2999226-x64-pkgProperties.txt
    |   |   |   |       Windows6.1-KB2999226-x64.cab
    |   |   |   |       Windows6.1-KB2999226-x64.xml
    |   |   |   |       WSUSSCAN.cab
    |   |   |   |       
    |   |   |   +---WOW64
    |   |   |   +---x64
    |   |   |   |   +---u..rsalcrt-apifwd-win7_6.1.7601.18972
    |   |   |   |   |       api-ms-win-core-file-l1-2-0.dll
    |   |   |   |   |       api-ms-win-core-file-l2-1-0.dll
    |   |   |   |   |       api-ms-win-core-localization-l1-2-0.dll
    |   |   |   |   |       api-ms-win-core-synch-l1-2-0.dll
    |   |   |   |   |       api-ms-win-core-timezone-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-xstate-l2-1-0.dll
    |   |   |   |   |       api-ms-win-crt-conio-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-convert-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-environment-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-filesystem-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-heap-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-locale-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-math-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-multibyte-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-private-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-process-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-runtime-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-stdio-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-string-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-time-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-utility-l1-1-0.dll
    |   |   |   |   |       api-ms-win-eventing-provider-l1-1-0.dll
    |   |   |   |   |       
    |   |   |   |   +---u..rsalcrt-apifwd-win7_6.1.7601.23175
    |   |   |   |   |       api-ms-win-core-file-l1-2-0.dll
    |   |   |   |   |       api-ms-win-core-file-l2-1-0.dll
    |   |   |   |   |       api-ms-win-core-localization-l1-2-0.dll
    |   |   |   |   |       api-ms-win-core-synch-l1-2-0.dll
    |   |   |   |   |       api-ms-win-core-timezone-l1-1-0.dll
    |   |   |   |   |       api-ms-win-core-xstate-l2-1-0.dll
    |   |   |   |   |       api-ms-win-crt-conio-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-convert-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-environment-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-filesystem-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-heap-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-locale-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-math-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-multibyte-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-private-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-process-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-runtime-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-stdio-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-string-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-time-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-utility-l1-1-0.dll
    |   |   |   |   |       api-ms-win-eventing-provider-l1-1-0.dll
    |   |   |   |   |       
    |   |   |   |   +---ucrt_6.1.7601.18972
    |   |   |   |   |       ucrtbase.dll
    |   |   |   |   |       
    |   |   |   |   \---ucrt_6.1.7601.23175
    |   |   |   |           ucrtbase.dll
    |   |   |   |           
    |   |   |   \---x86
    |   |   |       +---u..rsalcrt-apifwd-win7_6.1.7601.18972
    |   |   |       |       api-ms-win-core-file-l1-2-0.dll
    |   |   |       |       api-ms-win-core-file-l2-1-0.dll
    |   |   |       |       api-ms-win-core-localization-l1-2-0.dll
    |   |   |       |       api-ms-win-core-synch-l1-2-0.dll
    |   |   |       |       api-ms-win-core-timezone-l1-1-0.dll
    |   |   |       |       api-ms-win-core-xstate-l2-1-0.dll
    |   |   |       |       api-ms-win-crt-conio-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-convert-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-environment-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-filesystem-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-heap-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-locale-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-math-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-multibyte-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-private-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-process-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-runtime-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-stdio-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-string-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-time-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-utility-l1-1-0.dll
    |   |   |       |       api-ms-win-eventing-provider-l1-1-0.dll
    |   |   |       |       
    |   |   |       +---u..rsalcrt-apifwd-win7_6.1.7601.23175
    |   |   |       |       api-ms-win-core-file-l1-2-0.dll
    |   |   |       |       api-ms-win-core-file-l2-1-0.dll
    |   |   |       |       api-ms-win-core-localization-l1-2-0.dll
    |   |   |       |       api-ms-win-core-synch-l1-2-0.dll
    |   |   |       |       api-ms-win-core-timezone-l1-1-0.dll
    |   |   |       |       api-ms-win-core-xstate-l2-1-0.dll
    |   |   |       |       api-ms-win-crt-conio-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-convert-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-environment-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-filesystem-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-heap-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-locale-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-math-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-multibyte-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-private-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-process-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-runtime-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-stdio-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-string-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-time-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-utility-l1-1-0.dll
    |   |   |       |       api-ms-win-eventing-provider-l1-1-0.dll
    |   |   |       |       
    |   |   |       +---ucrt_6.1.7601.18972
    |   |   |       |       ucrtbase.dll
    |   |   |       |       
    |   |   |       \---ucrt_6.1.7601.23175
    |   |   |               ucrtbase.dll
    |   |   |               
    |   |   +---_Windows8-RT-KB2999226-x64.msu_
    |   |   |   +---JUNK
    |   |   |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.2.1.9.cat
    |   |   |   |       package_1_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.2.1.9.mum
    |   |   |   |       package_1_for_kb2999226~31bf3856ad364e35~amd64~~6.2.1.9.cat
    |   |   |   |       package_1_for_kb2999226~31bf3856ad364e35~amd64~~6.2.1.9.mum
    |   |   |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.2.1.9.cat
    |   |   |   |       package_2_for_kb2999226_bf~31bf3856ad364e35~amd64~~6.2.1.9.mum
    |   |   |   |       package_2_for_kb2999226~31bf3856ad364e35~amd64~~6.2.1.9.cat
    |   |   |   |       package_2_for_kb2999226~31bf3856ad364e35~amd64~~6.2.1.9.mum
    |   |   |   |       package_for_kb2999226_rtm_bf~31bf3856ad364e35~amd64~~6.2.1.9.cat
    |   |   |   |       package_for_kb2999226_rtm_bf~31bf3856ad364e35~amd64~~6.2.1.9.mum
    |   |   |   |       package_for_kb2999226_rtm~31bf3856ad364e35~amd64~~6.2.1.9.cat
    |   |   |   |       package_for_kb2999226_rtm~31bf3856ad364e35~amd64~~6.2.1.9.mum
    |   |   |   |       update-bf.cat
    |   |   |   |       update-bf.mum
    |   |   |   |       update.cat
    |   |   |   |       update.mum
    |   |   |   |       
    |   |   |   +---MSIL
    |   |   |   +---PATCH
    |   |   |   |       Windows8-RT-KB2999226-x64-pkgProperties.txt
    |   |   |   |       Windows8-RT-KB2999226-x64.cab
    |   |   |   |       Windows8-RT-KB2999226-x64.xml
    |   |   |   |       WSUSSCAN.cab
    |   |   |   |       
    |   |   |   +---WOW64
    |   |   |   +---x64
    |   |   |   |   +---u..rsalcrt-apifwd-win8_6.2.9200.17488
    |   |   |   |   |       api-ms-win-core-xstate-l2-1-0.dll
    |   |   |   |   |       api-ms-win-crt-conio-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-convert-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-environment-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-filesystem-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-heap-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-locale-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-math-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-multibyte-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-private-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-process-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-runtime-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-stdio-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-string-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-time-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-utility-l1-1-0.dll
    |   |   |   |   |       api-ms-win-eventing-provider-l1-1-0.dll
    |   |   |   |   |       
    |   |   |   |   +---u..rsalcrt-apifwd-win8_6.2.9200.21602
    |   |   |   |   |       api-ms-win-core-xstate-l2-1-0.dll
    |   |   |   |   |       api-ms-win-crt-conio-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-convert-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-environment-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-filesystem-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-heap-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-locale-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-math-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-multibyte-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-private-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-process-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-runtime-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-stdio-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-string-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-time-l1-1-0.dll
    |   |   |   |   |       api-ms-win-crt-utility-l1-1-0.dll
    |   |   |   |   |       api-ms-win-eventing-provider-l1-1-0.dll
    |   |   |   |   |       
    |   |   |   |   +---ucrt_6.2.9200.17488
    |   |   |   |   |       ucrtbase.dll
    |   |   |   |   |       
    |   |   |   |   \---ucrt_6.2.9200.21602
    |   |   |   |           ucrtbase.dll
    |   |   |   |           
    |   |   |   \---x86
    |   |   |       +---u..rsalcrt-apifwd-win8_6.2.9200.17488
    |   |   |       |       api-ms-win-core-xstate-l2-1-0.dll
    |   |   |       |       api-ms-win-crt-conio-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-convert-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-environment-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-filesystem-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-heap-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-locale-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-math-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-multibyte-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-private-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-process-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-runtime-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-stdio-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-string-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-time-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-utility-l1-1-0.dll
    |   |   |       |       api-ms-win-eventing-provider-l1-1-0.dll
    |   |   |       |       
    |   |   |       +---u..rsalcrt-apifwd-win8_6.2.9200.21602
    |   |   |       |       api-ms-win-core-xstate-l2-1-0.dll
    |   |   |       |       api-ms-win-crt-conio-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-convert-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-environment-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-filesystem-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-heap-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-locale-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-math-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-multibyte-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-private-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-process-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-runtime-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-stdio-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-string-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-time-l1-1-0.dll
    |   |   |       |       api-ms-win-crt-utility-l1-1-0.dll
    |   |   |       |       api-ms-win-eventing-provider-l1-1-0.dll
    |   |   |       |       
    |   |   |       +---ucrt_6.2.9200.17488
    |   |   |       |       ucrtbase.dll
    |   |   |       |       
    |   |   |       \---ucrt_6.2.9200.21602
    |   |   |               ucrtbase.dll
    |   |   |               
    |   |   \---_Windows8.1-KB2999226-x64.msu_
    |   |       +---JUNK
    |   |       |       package_1_for_kb2999226~31bf3856ad364e35~amd64~~6.3.1.9.cat
    |   |       |       package_1_for_kb2999226~31bf3856ad364e35~amd64~~6.3.1.9.mum
    |   |       |       package_for_kb2999226_rtm_gm~31bf3856ad364e35~amd64~~6.3.1.9.cat
    |   |       |       package_for_kb2999226_rtm_gm~31bf3856ad364e35~amd64~~6.3.1.9.mum
    |   |       |       package_for_kb2999226_rtm~31bf3856ad364e35~amd64~~6.3.1.9.cat
    |   |       |       package_for_kb2999226_rtm~31bf3856ad364e35~amd64~~6.3.1.9.mum
    |   |       |       update.cat
    |   |       |       update.mum
    |   |       |       
    |   |       +---MSIL
    |   |       +---PATCH
    |   |       |       Windows8.1-KB2999226-x64-pkgProperties.txt
    |   |       |       Windows8.1-KB2999226-x64.cab
    |   |       |       Windows8.1-KB2999226-x64.xml
    |   |       |       WSUSSCAN.cab
    |   |       |       
    |   |       +---WOW64
    |   |       +---x64
    |   |       |   +---u..lcrt-apifwd-winblue_6.3.9600.18036
    |   |       |   |       api-ms-win-crt-conio-l1-1-0.dll
    |   |       |   |       api-ms-win-crt-convert-l1-1-0.dll
    |   |       |   |       api-ms-win-crt-environment-l1-1-0.dll
    |   |       |   |       api-ms-win-crt-filesystem-l1-1-0.dll
    |   |       |   |       api-ms-win-crt-heap-l1-1-0.dll
    |   |       |   |       api-ms-win-crt-locale-l1-1-0.dll
    |   |       |   |       api-ms-win-crt-math-l1-1-0.dll
    |   |       |   |       api-ms-win-crt-multibyte-l1-1-0.dll
    |   |       |   |       api-ms-win-crt-private-l1-1-0.dll
    |   |       |   |       api-ms-win-crt-process-l1-1-0.dll
    |   |       |   |       api-ms-win-crt-runtime-l1-1-0.dll
    |   |       |   |       api-ms-win-crt-stdio-l1-1-0.dll
    |   |       |   |       api-ms-win-crt-string-l1-1-0.dll
    |   |       |   |       api-ms-win-crt-time-l1-1-0.dll
    |   |       |   |       api-ms-win-crt-utility-l1-1-0.dll
    |   |       |   |       
    |   |       |   \---ucrt_6.3.9600.18036
    |   |       |           ucrtbase.dll
    |   |       |           
    |   |       \---x86
    |   |           +---u..lcrt-apifwd-winblue_6.3.9600.18036
    |   |           |       api-ms-win-crt-conio-l1-1-0.dll
    |   |           |       api-ms-win-crt-convert-l1-1-0.dll
    |   |           |       api-ms-win-crt-environment-l1-1-0.dll
    |   |           |       api-ms-win-crt-filesystem-l1-1-0.dll
    |   |           |       api-ms-win-crt-heap-l1-1-0.dll
    |   |           |       api-ms-win-crt-locale-l1-1-0.dll
    |   |           |       api-ms-win-crt-math-l1-1-0.dll
    |   |           |       api-ms-win-crt-multibyte-l1-1-0.dll
    |   |           |       api-ms-win-crt-private-l1-1-0.dll
    |   |           |       api-ms-win-crt-process-l1-1-0.dll
    |   |           |       api-ms-win-crt-runtime-l1-1-0.dll
    |   |           |       api-ms-win-crt-stdio-l1-1-0.dll
    |   |           |       api-ms-win-crt-string-l1-1-0.dll
    |   |           |       api-ms-win-crt-time-l1-1-0.dll
    |   |           |       api-ms-win-crt-utility-l1-1-0.dll
    |   |           |       
    |   |           \---ucrt_6.3.9600.18036
    |   |                   ucrtbase.dll
    |   |                   
    |   \---x86
    |       +---_Windows6.0-KB2999226-x86.msu_
    |       |   \---x86
    |       |       +---u..salcrt-apifwd-vista_6.0.6002.19488
    |       |       |       api-ms-win-core-console-l1-1-0.dll
    |       |       |       api-ms-win-core-datetime-l1-1-0.dll
    |       |       |       api-ms-win-core-debug-l1-1-0.dll
    |       |       |       api-ms-win-core-errorhandling-l1-1-0.dll
    |       |       |       api-ms-win-core-file-l1-1-0.dll
    |       |       |       api-ms-win-core-file-l1-2-0.dll
    |       |       |       api-ms-win-core-file-l2-1-0.dll
    |       |       |       api-ms-win-core-handle-l1-1-0.dll
    |       |       |       api-ms-win-core-heap-l1-1-0.dll
    |       |       |       api-ms-win-core-interlocked-l1-1-0.dll
    |       |       |       api-ms-win-core-libraryloader-l1-1-0.dll
    |       |       |       api-ms-win-core-localization-l1-2-0.dll
    |       |       |       api-ms-win-core-memory-l1-1-0.dll
    |       |       |       api-ms-win-core-namedpipe-l1-1-0.dll
    |       |       |       api-ms-win-core-profile-l1-1-0.dll
    |       |       |       api-ms-win-core-rtlsupport-l1-1-0.dll
    |       |       |       api-ms-win-core-string-l1-1-0.dll
    |       |       |       api-ms-win-core-synch-l1-1-0.dll
    |       |       |       api-ms-win-core-synch-l1-2-0.dll
    |       |       |       api-ms-win-core-sysinfo-l1-1-0.dll
    |       |       |       api-ms-win-core-timezone-l1-1-0.dll
    |       |       |       api-ms-win-core-util-l1-1-0.dll
    |       |       |       api-ms-win-core-xstate-l2-1-0.dll
    |       |       |       api-ms-win-crt-conio-l1-1-0.dll
    |       |       |       api-ms-win-crt-convert-l1-1-0.dll
    |       |       |       api-ms-win-crt-environment-l1-1-0.dll
    |       |       |       api-ms-win-crt-filesystem-l1-1-0.dll
    |       |       |       api-ms-win-crt-heap-l1-1-0.dll
    |       |       |       api-ms-win-crt-locale-l1-1-0.dll
    |       |       |       api-ms-win-crt-math-l1-1-0.dll
    |       |       |       api-ms-win-crt-multibyte-l1-1-0.dll
    |       |       |       api-ms-win-crt-private-l1-1-0.dll
    |       |       |       api-ms-win-crt-process-l1-1-0.dll
    |       |       |       api-ms-win-crt-runtime-l1-1-0.dll
    |       |       |       api-ms-win-crt-stdio-l1-1-0.dll
    |       |       |       api-ms-win-crt-string-l1-1-0.dll
    |       |       |       api-ms-win-crt-time-l1-1-0.dll
    |       |       |       api-ms-win-crt-utility-l1-1-0.dll
    |       |       |       api-ms-win-eventing-provider-l1-1-0.dll
    |       |       |       
    |       |       +---u..salcrt-apifwd-vista_6.0.6002.23798
    |       |       |       api-ms-win-core-console-l1-1-0.dll
    |       |       |       api-ms-win-core-datetime-l1-1-0.dll
    |       |       |       api-ms-win-core-debug-l1-1-0.dll
    |       |       |       api-ms-win-core-errorhandling-l1-1-0.dll
    |       |       |       api-ms-win-core-file-l1-1-0.dll
    |       |       |       api-ms-win-core-file-l1-2-0.dll
    |       |       |       api-ms-win-core-file-l2-1-0.dll
    |       |       |       api-ms-win-core-handle-l1-1-0.dll
    |       |       |       api-ms-win-core-heap-l1-1-0.dll
    |       |       |       api-ms-win-core-interlocked-l1-1-0.dll
    |       |       |       api-ms-win-core-libraryloader-l1-1-0.dll
    |       |       |       api-ms-win-core-localization-l1-2-0.dll
    |       |       |       api-ms-win-core-memory-l1-1-0.dll
    |       |       |       api-ms-win-core-namedpipe-l1-1-0.dll
    |       |       |       api-ms-win-core-profile-l1-1-0.dll
    |       |       |       api-ms-win-core-rtlsupport-l1-1-0.dll
    |       |       |       api-ms-win-core-string-l1-1-0.dll
    |       |       |       api-ms-win-core-synch-l1-1-0.dll
    |       |       |       api-ms-win-core-synch-l1-2-0.dll
    |       |       |       api-ms-win-core-sysinfo-l1-1-0.dll
    |       |       |       api-ms-win-core-timezone-l1-1-0.dll
    |       |       |       api-ms-win-core-util-l1-1-0.dll
    |       |       |       api-ms-win-core-xstate-l2-1-0.dll
    |       |       |       api-ms-win-crt-conio-l1-1-0.dll
    |       |       |       api-ms-win-crt-convert-l1-1-0.dll
    |       |       |       api-ms-win-crt-environment-l1-1-0.dll
    |       |       |       api-ms-win-crt-filesystem-l1-1-0.dll
    |       |       |       api-ms-win-crt-heap-l1-1-0.dll
    |       |       |       api-ms-win-crt-locale-l1-1-0.dll
    |       |       |       api-ms-win-crt-math-l1-1-0.dll
    |       |       |       api-ms-win-crt-multibyte-l1-1-0.dll
    |       |       |       api-ms-win-crt-private-l1-1-0.dll
    |       |       |       api-ms-win-crt-process-l1-1-0.dll
    |       |       |       api-ms-win-crt-runtime-l1-1-0.dll
    |       |       |       api-ms-win-crt-stdio-l1-1-0.dll
    |       |       |       api-ms-win-crt-string-l1-1-0.dll
    |       |       |       api-ms-win-crt-time-l1-1-0.dll
    |       |       |       api-ms-win-crt-utility-l1-1-0.dll
    |       |       |       api-ms-win-eventing-provider-l1-1-0.dll
    |       |       |       
    |       |       +---ucrt_6.0.6002.19488
    |       |       |       ucrtbase.dll
    |       |       |       
    |       |       \---ucrt_6.0.6002.23798
    |       |               ucrtbase.dll
    |       |               
    |       +---_Windows6.1-KB2999226-x86.msu_
    |       |   \---x86
    |       |       +---u..rsalcrt-apifwd-win7_6.1.7601.18972
    |       |       |       api-ms-win-core-file-l1-2-0.dll
    |       |       |       api-ms-win-core-file-l2-1-0.dll
    |       |       |       api-ms-win-core-localization-l1-2-0.dll
    |       |       |       api-ms-win-core-synch-l1-2-0.dll
    |       |       |       api-ms-win-core-timezone-l1-1-0.dll
    |       |       |       api-ms-win-core-xstate-l2-1-0.dll
    |       |       |       api-ms-win-crt-conio-l1-1-0.dll
    |       |       |       api-ms-win-crt-convert-l1-1-0.dll
    |       |       |       api-ms-win-crt-environment-l1-1-0.dll
    |       |       |       api-ms-win-crt-filesystem-l1-1-0.dll
    |       |       |       api-ms-win-crt-heap-l1-1-0.dll
    |       |       |       api-ms-win-crt-locale-l1-1-0.dll
    |       |       |       api-ms-win-crt-math-l1-1-0.dll
    |       |       |       api-ms-win-crt-multibyte-l1-1-0.dll
    |       |       |       api-ms-win-crt-private-l1-1-0.dll
    |       |       |       api-ms-win-crt-process-l1-1-0.dll
    |       |       |       api-ms-win-crt-runtime-l1-1-0.dll
    |       |       |       api-ms-win-crt-stdio-l1-1-0.dll
    |       |       |       api-ms-win-crt-string-l1-1-0.dll
    |       |       |       api-ms-win-crt-time-l1-1-0.dll
    |       |       |       api-ms-win-crt-utility-l1-1-0.dll
    |       |       |       api-ms-win-eventing-provider-l1-1-0.dll
    |       |       |       
    |       |       +---u..rsalcrt-apifwd-win7_6.1.7601.23175
    |       |       |       api-ms-win-core-file-l1-2-0.dll
    |       |       |       api-ms-win-core-file-l2-1-0.dll
    |       |       |       api-ms-win-core-localization-l1-2-0.dll
    |       |       |       api-ms-win-core-synch-l1-2-0.dll
    |       |       |       api-ms-win-core-timezone-l1-1-0.dll
    |       |       |       api-ms-win-core-xstate-l2-1-0.dll
    |       |       |       api-ms-win-crt-conio-l1-1-0.dll
    |       |       |       api-ms-win-crt-convert-l1-1-0.dll
    |       |       |       api-ms-win-crt-environment-l1-1-0.dll
    |       |       |       api-ms-win-crt-filesystem-l1-1-0.dll
    |       |       |       api-ms-win-crt-heap-l1-1-0.dll
    |       |       |       api-ms-win-crt-locale-l1-1-0.dll
    |       |       |       api-ms-win-crt-math-l1-1-0.dll
    |       |       |       api-ms-win-crt-multibyte-l1-1-0.dll
    |       |       |       api-ms-win-crt-private-l1-1-0.dll
    |       |       |       api-ms-win-crt-process-l1-1-0.dll
    |       |       |       api-ms-win-crt-runtime-l1-1-0.dll
    |       |       |       api-ms-win-crt-stdio-l1-1-0.dll
    |       |       |       api-ms-win-crt-string-l1-1-0.dll
    |       |       |       api-ms-win-crt-time-l1-1-0.dll
    |       |       |       api-ms-win-crt-utility-l1-1-0.dll
    |       |       |       api-ms-win-eventing-provider-l1-1-0.dll
    |       |       |       
    |       |       +---ucrt_6.1.7601.18972
    |       |       |       ucrtbase.dll
    |       |       |       
    |       |       \---ucrt_6.1.7601.23175
    |       |               ucrtbase.dll
    |       |               
    |       +---_Windows8-RT-KB2999226-x86.msu_
    |       |   \---x86
    |       |       +---u..rsalcrt-apifwd-win8_6.2.9200.17488
    |       |       |       api-ms-win-core-xstate-l2-1-0.dll
    |       |       |       api-ms-win-crt-conio-l1-1-0.dll
    |       |       |       api-ms-win-crt-convert-l1-1-0.dll
    |       |       |       api-ms-win-crt-environment-l1-1-0.dll
    |       |       |       api-ms-win-crt-filesystem-l1-1-0.dll
    |       |       |       api-ms-win-crt-heap-l1-1-0.dll
    |       |       |       api-ms-win-crt-locale-l1-1-0.dll
    |       |       |       api-ms-win-crt-math-l1-1-0.dll
    |       |       |       api-ms-win-crt-multibyte-l1-1-0.dll
    |       |       |       api-ms-win-crt-private-l1-1-0.dll
    |       |       |       api-ms-win-crt-process-l1-1-0.dll
    |       |       |       api-ms-win-crt-runtime-l1-1-0.dll
    |       |       |       api-ms-win-crt-stdio-l1-1-0.dll
    |       |       |       api-ms-win-crt-string-l1-1-0.dll
    |       |       |       api-ms-win-crt-time-l1-1-0.dll
    |       |       |       api-ms-win-crt-utility-l1-1-0.dll
    |       |       |       api-ms-win-eventing-provider-l1-1-0.dll
    |       |       |       
    |       |       +---u..rsalcrt-apifwd-win8_6.2.9200.21602
    |       |       |       api-ms-win-core-xstate-l2-1-0.dll
    |       |       |       api-ms-win-crt-conio-l1-1-0.dll
    |       |       |       api-ms-win-crt-convert-l1-1-0.dll
    |       |       |       api-ms-win-crt-environment-l1-1-0.dll
    |       |       |       api-ms-win-crt-filesystem-l1-1-0.dll
    |       |       |       api-ms-win-crt-heap-l1-1-0.dll
    |       |       |       api-ms-win-crt-locale-l1-1-0.dll
    |       |       |       api-ms-win-crt-math-l1-1-0.dll
    |       |       |       api-ms-win-crt-multibyte-l1-1-0.dll
    |       |       |       api-ms-win-crt-private-l1-1-0.dll
    |       |       |       api-ms-win-crt-process-l1-1-0.dll
    |       |       |       api-ms-win-crt-runtime-l1-1-0.dll
    |       |       |       api-ms-win-crt-stdio-l1-1-0.dll
    |       |       |       api-ms-win-crt-string-l1-1-0.dll
    |       |       |       api-ms-win-crt-time-l1-1-0.dll
    |       |       |       api-ms-win-crt-utility-l1-1-0.dll
    |       |       |       api-ms-win-eventing-provider-l1-1-0.dll
    |       |       |       
    |       |       +---ucrt_6.2.9200.17488
    |       |       |       ucrtbase.dll
    |       |       |       
    |       |       \---ucrt_6.2.9200.21602
    |       |               ucrtbase.dll
    |       |               
    |       \---_Windows8.1-KB2999226-x86.msu_
    |           \---x86
    |               +---u..lcrt-apifwd-winblue_6.3.9600.18036
    |               |       api-ms-win-crt-conio-l1-1-0.dll
    |               |       api-ms-win-crt-convert-l1-1-0.dll
    |               |       api-ms-win-crt-environment-l1-1-0.dll
    |               |       api-ms-win-crt-filesystem-l1-1-0.dll
    |               |       api-ms-win-crt-heap-l1-1-0.dll
    |               |       api-ms-win-crt-locale-l1-1-0.dll
    |               |       api-ms-win-crt-math-l1-1-0.dll
    |               |       api-ms-win-crt-multibyte-l1-1-0.dll
    |               |       api-ms-win-crt-private-l1-1-0.dll
    |               |       api-ms-win-crt-process-l1-1-0.dll
    |               |       api-ms-win-crt-runtime-l1-1-0.dll
    |               |       api-ms-win-crt-stdio-l1-1-0.dll
    |               |       api-ms-win-crt-string-l1-1-0.dll
    |               |       api-ms-win-crt-time-l1-1-0.dll
    |               |       api-ms-win-crt-utility-l1-1-0.dll
    |               |       
    |               \---ucrt_6.3.9600.18036
    |                       ucrtbase.dll
    |                       
    +---vc_runtimeAdditional_x86
    |   |   vc_runtimeAdditional_x86.msi
    |   |   
    |   \---System
    |           mfc140.dll
    |           mfc140chs.dll
    |           mfc140cht.dll
    |           mfc140deu.dll
    |           mfc140enu.dll
    |           mfc140esn.dll
    |           mfc140fra.dll
    |           mfc140ita.dll
    |           mfc140jpn.dll
    |           mfc140kor.dll
    |           mfc140rus.dll
    |           mfc140u.dll
    |           mfcm140.dll
    |           mfcm140u.dll
    |           
    \---vc_runtimeMinimum_x86
        |   vc_runtimeMinimum_x86.msi
        |   
        \---System
                concrt140.dll
                msvcp140.dll
                msvcp140_1.dll
                msvcp140_2.dll
                msvcp140_atomic_wait.dll
                msvcp140_codecvt_ids.dll
                vcamp140.dll
                vccorlib140.dll
                vcomp140.dll
                vcruntime140.dll

```

</details>

<hr/>
<br/>

note:  
you can copy dlls directly,  
but for installations or embedding: it is best to download the zip files.  
the zip files were archived on a Windows machine, and unlike GitHub stored files,  
xml, manifest, and ini files would preserve their Windows end-of-line character.  

note:  
this repository was constructed so you won't have/need to look around shady or malicious websites for those DLLs.  
when people really need to run a program, they get desperate enough to skip through various "website isn't safe",  
and download mystery files (and run them), thus putting themselves at risk of spywares, rootkits and plain viruses.  
I hope this humble repository would help in some way.  
you can link to this repository, fork or download it.  
<a title="buy me a cup of coffee » ☕︎ (optional)" href="https://%70%61%79%70%61%6C%2E%6D%65/%65%31%61%64%6B%61%72%61%6B%30/%35%55%53%44">»☕︎«</a>  

<br/>
<br/>
<hr/>

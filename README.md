# Course_bigdata
NTUST Course Big Data Analytics HW1

# 作業說明

#### 1. 哪些屬性對於惡意程式分類有效?  
前10重要的屬性：  
dc_por    
TB_b9   
ent_q_diff_diffs_1_median   
LCMapStringA   
TB_e5   
Img0.1   
ent_q_diff_diffs_1_min   
_allmul   
ent_q_diff_diffs_2_median   
TB_7b    
    
#### 2. 哪些屬性對於惡意程式分類無效?   
最不重要的100個屬性：  
FileTimeToSystemTime  
FileTimeToLocalFileTime  
ExtTextOutA  
ExpandEnvironmentStringsA  
ExitWindowsEx  
Escape  
EqualRect  
EnumThreadWindows  
EnumChildWindows  
EnumCalendarInfoA  
EndPaint  
EndDialog  
EnableWindow  
EnableScrollBar  
EnableMenuItem  
EmptyClipboard  
EVENT_SINK_AddRef  
DuplicateHandle  
DrawIconEx  
DrawIcon  
DrawFrameControl  
DrawFocusRect  
DrawEdge  
DllFunctionCall  
DispatchMessageW  
DispatchMessageA  
DisableThreadLibraryCalls  
DeviceIoControl  
DestroyMenu  
DestroyIcon  
DestroyCursor  
DeleteService  
DeleteMenu  
DeleteFileW  
DeleteEnhMetaFile  
DefWindowProcW  
DefWindowProcA  
DefMDIChildProcA  
DefFrameProcA  
CreateWindowExW   
CreateServiceA  
CreateRemoteThread  
CreateRectRgn   
CreateProcessW  
CreatePopupMenu  
CreatePipe   
CreatePenIndirect  
CreatePalette  
CreateMenu  
CreateIcon  
CreateHalftonePalette  
CreateFontIndirectA  
CreateFileW  
CreateFileMappingA  
CreateEventW  
CreateDirectoryW  
CreateDialogParamA  
CreateDIBitmap  
CreateDCA  
CreateCompatibleBitmap  
CreateBrushIndirect  
CreateBitmap  
CopyFileA  
CopyEnhMetaFileA  
ControlService  
CompareStringW  
CompareFileTime  
CoUninitialize  
CoTaskMemFree  
CoTaskMemAlloc  
CoInitialize  
CoGetClassObject  
ClosePrinter  
CloseClipboard  
ClientToScreen  
CheckMenuItem  
CheckDlgButton  
CharUpperBuffA  
CharUpperA  
CharToOemA  
CharPrevA  
CharNextW  
CharNextA  
CharLowerBuffA  
CharLowerA  
CallWindowProcA  
CallNextHookEx  
CLSIDFromString  
CLSIDFromProgID  
BringWindowToTop  
BitBlt  
BeginPaint  
BASS  
AppendMenuA  
AdjustWindowRectEx  
AdjustTokenPrivileges  
ActivateKeyboardLayout  
.tls_por  
.edata_por  
*invalid*  
    
#### 3. 用什麼方法可以幫助你決定上述的結論?   
用random forest演算法, 將全部features丟入模型根據給的label進行分類, 最後得出各個feature 的重要性   
     
#### 4. 透過Python哪些套件以及方法可以幫助你完成上面的工作?   
sklearn, pandas, numpy, random forest classifier  
     
#### 5. 課程迄今有無建議?(老師教學風趣或良好就不用再提囉)
無，非常好

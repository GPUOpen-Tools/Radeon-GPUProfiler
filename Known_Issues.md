# Known Issues

1)  Radeon Developer Panel will NOT capture profiles from AMD multi-GPU configurations (e.g. two AMD GPUs).
    It will work with one AMD GPU and other competitor cards installed in the same machine. Please note that the primary monitor will need to be configured for the AMD GPU/monitor combination.
2)  Radeon Developer Panel can only capture a profile on a single AMD GPU at a time.
3)  Radeon Developer Panel cannot capture profiles from competitor GPUs.
4)  Radeon Developer Panel will NOT capture profiles from Windows Insider Editions.
5)  Anti-virus may impede key-based capture (Ctrl+Shift+C)
6)  There are no driver settings available for Vulkan yet.
7)  Applications that call Present() from the async compute queue are not supported. A fix will be available soon.
8)  Queue synchronization data will be missing from DirectX12 apps running on Windows 10 Home.
9)  If the Developer Panel or the Developer Service crash on Linux while running with the root account, it may be necessary to restart/exit them again with the root account in order to cleanup shared memory.
10) On Linux, the Radeon Developer Service and Panel are only officially supported using the standard desktop managers (GDM and Unity). Other desktop managers should work but a dialog box indicating that the service is running in headless mode may pop up. However, it should still be possible to capture profiles.
11) If the RadeonDeveloperServiceCLI application crashes on Linux, shared memory may need to be cleaned up by running the RemoveSharedMemory.sh script located in the script folder of the RGP release kit. Run the script with elevated privileges using sudo.
12) On Linux, the Radeon Developer Panel may fail to start the Radeon Developer Service when the Connect button is clicked. If this occurs, manually start the Radeon Developer Service, select localhost from the the Recent connections list and click the Connect button again.
13) Raven Ridge APU's are not currently supported.
14) D3D12 command list calls of ExecuteIndirect() may show in RGP as multiple compute events. This will be corrected in a future release after obtaining more information from the driver.
15) The Radeon Overlay hotkey, Alt+R, conflicts with the Radeon GPU Profiler shortcut key used to select the Pipeline state pane.  The Radeon Overlay hotkey can be reconfigured by opening the Radeon Settings panel (from the system tray), selecting the Preferences tab then clicking the "Toggle Radeon Overlay Hotkey" button.

- [x] void InitWindow(int width, int height, const char *title); # Implemented: `new Window`
- [x] void CloseWindow(void); # Implemented: `Window = null`
- [x] bool WindowShouldClose(void); # Implemented: `Window.should_close`
- [x] bool IsWindowReady(void); # Implemented: `Window.ready`
- [x] bool IsWindowFullscreen(void); # Implemented: `Window.fullscreen`
- [x] bool IsWindowHidden(void); # Implemented: `Window.hidden`
- [x] bool IsWindowMinimized(void); # Implemented: `Window.minimized`
- [x] bool IsWindowMaximized(void); # Implemented: `Window.maximized`
- [x] bool IsWindowFocused(void); # Implemented: `Window.focused`
- [x] bool IsWindowResized(void); # Implemented: `Window.resized`
- ❌ bool IsWindowState(unsigned int flag); # Unneeded
- ❌ void SetWindowState(unsigned int flags); # Unneeded
- ❌ void ClearWindowState(unsigned int flags); # Unneeded
- [x] void ToggleFullscreen(void); # Implemented: `Window.fullscreen`
- [x] void ToggleBorderlessWindowed(void); # Implemented: `Window.borderless`
- [x] void MaximizeWindow(void); # Implemented: `Window.maximized`
- [x] void MinimizeWindow(void); # Implemented: `Window.minimized`
- [x] void RestoreWindow(void); # Implemented: `Window.restore`
- [ ] void SetWindowIcon(Image image);
- [ ] void SetWindowIcons(Image *images, int count);
- [x] void SetWindowTitle(const char *title); # Implemented: `Window.title`
- [x] void SetWindowPosition(int x, int y); # Implemented: `Window.position`
- [ ] void SetWindowMonitor(int monitor);
- [x] void SetWindowMinSize(int width, int height); # Implemented: `Window.minimum_width` and `Window.minimum_height`
- [ ] void SetWindowMaxSize(int width, int height);
- [x] void SetWindowSize(int width, int height); # Implemented: `Window.width` and `Window.height`
- [ ] void SetWindowOpacity(float opacity);
- [ ] void SetWindowFocused(void);
- [ ] void *GetWindowHandle(void);
- [x] int GetScreenWidth(void); # Implemented: `Window.width`
- [x] int GetScreenHeight(void); # Implemented: `Window.height`
- [ ] int GetRenderWidth(void);
- [ ] int GetRenderHeight(void);
- [x] int GetMonitorCount(void); # Implemented: `Window.monitors.length`
- [x] int GetCurrentMonitor(void); # Implemented: `Window.get_current_monitor`
- [ ] Vector2 GetMonitorPosition(int monitor);
- [x] int GetMonitorWidth(int monitor);  # Implemented: `Window.monitors[x].width`
- [x] int GetMonitorHeight(int monitor);  # Implemented: `Window.monitors[x].height`
- [x] int GetMonitorPhysicalWidth(int monitor); # Implemented: `Window.monitors[x].physical_width`
- [x] int GetMonitorPhysicalHeight(int monitor); # Implemented: `Window.monitors[x].physical_height`
- [x] int GetMonitorRefreshRate(int monitor); # Implemented: `Window.monitors[x].refresh_rate`
- [x] Vector2 GetWindowPosition(void); # Implemented: `Window.position`
- [ ] Vector2 GetWindowScaleDPI(void);
- [x] const char *GetMonitorName(int monitor); # Implemented: `Window.monitors[x].name`
- [x] void SetClipboardText(const char *text); # Implemented: `Clipboard.set`
- [x] const char *GetClipboardText(void); # Implemented: `Clipboard.get`
- [x] void EnableEventWaiting(void); # Implemented: `Window.event_waiting`
- [x] void DisableEventWaiting(void); # Implemented: `Window.event_waiting`
- [x] void ShowCursor(void); # Implemented: `Window.Cursor.hidden`
- [x] void HideCursor(void); # Implemented: `Window.Cursor.hidden`
- [x] bool IsCursorHidden(void); # Implemented: `Window.Cursor.hidden`
- [x] void EnableCursor(void); # Implemented: `Window.Cursor.locked`
- [x] void DisableCursor(void); # Implemented: `Window.Cursor.locked`
- [x] bool IsCursorOnScreen(void); # Implemented: `Window.Cursor.on_screen`
- [x] void ClearBackground(Color color); # Implemented: `Window.clear_background`
- [x] void BeginDrawing(void); # Implemented: `Window.begin_drawing` and `Window.draw`
- [x] void EndDrawing(void); # Implemented: `Window.end_drawing` and `Window.draw`
- [x] void BeginMode2D(Camera2D camera); # Implemented: `Window.begin_2D`
- [x] void EndMode2D(void); # Implemented: `Window.end_2D`
- [ ] void BeginMode3D(Camera3D camera);
- [ ] void EndMode3D(void);
- [ ] void BeginTextureMode(RenderTexture2D target);
- [ ] void EndTextureMode(void);
- [ ] void BeginShaderMode(Shader shader);
- [ ] void EndShaderMode(void);
- [ ] void BeginBlendMode(int mode);
- [ ] void EndBlendMode(void);
- [x] void BeginScissorMode(int x, int y, int width, int height); # Implemented: `Window.begin_scissor` & `Window.scissor`
- [x] void EndScissorMode(void); # Implemented: `Window.begin_scissor` & `Window.scissor`
- [ ] void BeginVrStereoMode(VrStereoConfig config);
- [ ] void EndVrStereoMode(void);
- [ ] VrStereoConfig LoadVrStereoConfig(VrDeviceInfo device);
- [ ] void UnloadVrStereoConfig(VrStereoConfig config);
- [ ] Shader LoadShader(const char *vsFileName, const char *fsFileName);
- [ ] Shader LoadShaderFromMemory(const char *vsCode, const char *fsCode);
- [ ] bool IsShaderReady(Shader shader);
- [ ] int GetShaderLocation(Shader shader, const char *uniformName);
- [ ] int GetShaderLocationAttrib(Shader shader, const char *attribName);
- [ ] void SetShaderValue(Shader shader, int locIndex, const void *value, int uniformType);
- [ ] void SetShaderValueV(Shader shader, int locIndex, const void *value, int uniformType, int count);
- [ ] void SetShaderValueMatrix(Shader shader, int locIndex, Matrix mat);
- [ ] void SetShaderValueTexture(Shader shader, int locIndex, Texture2D texture);
- [ ] void UnloadShader(Shader shader);
- [ ] Ray GetMouseRay(Vector2 mousePosition, Camera camera);
- [ ] Matrix GetCameraMatrix(Camera camera);
- [ ] Matrix GetCameraMatrix2D(Camera2D camera);
- [ ] Vector2 GetWorldToScreen(Vector3 position, Camera camera);
- [ ] Vector2 GetScreenToWorld2D(Vector2 position, Camera2D camera);
- [ ] Vector2 GetWorldToScreenEx(Vector3 position, Camera camera, int width, int height);
- [ ] Vector2 GetWorldToScreen2D(Vector2 position, Camera2D camera);
- [x] void SetTargetFPS(int fps); # Implemented: `Window.target_fps`
- [x] float GetFrameTime(void); # Implemented: `Window.frame_time`
- [x] double GetTime(void); # Implemented: `Window.time`
- [x] int GetFPS(void); # Implemented: `Window.fps`
- [ ] void SwapScreenBuffer(void);
- [ ] void PollInputEvents(void);
- ❌ void WaitTime(double seconds); # Unneeded: Built-in to GLib `Thread.usleep`
- ❌ void SetRandomSeed(unsigned int seed); # Unneeded: Built-in to GLib `GLib.Random`
- ❌ int GetRandomValue(int min, int max); # Unneeded: Built-in to GLib `GLib.Random`
- ❌ int *LoadRandomSequence(unsigned int count, int min, int max); # Unneeded: Built-in to GLib `GLib.Random`
- ❌ void UnloadRandomSequence(int *sequence); # Unneeded: Built-in to GLib `GLib.Random`
- [x] void TakeScreenshot(const char *fileName); # Implemented: `Window.take_screenshot`
- [ ] void SetConfigFlags(unsigned int flags);
- ❌ void OpenURL(const char *url); # Unneeded: Built-in to GLib `GLib.AppInfo` and `GLib.AppLaunchContext`
- ❌ void TraceLog(int logLevel, const char *text, ...); # Unneeded: Builtin `GLib Log Functions`
- ❌ void SetTraceLogLevel(int logLevel); # Unneeded: Builtin `GLib Log Functions`
- ❌ void *MemAlloc(unsigned int size); # Unneeded: Built-in to GLib `GLib.malloc`
- ❌ void *MemRealloc(void *ptr, unsigned int size); # Unneeded: Built-in to GLib `GLib.realloc`
- ❌ void MemFree(void *ptr); # Unneeded: Built-in to GLib `GLib.free`
- ❌ void SetTraceLogCallback(TraceLogCallback callback); # Unneeded: Builtin `GLib Log Functions`
- ❌ void SetLoadFileDataCallback(LoadFileDataCallback callback); # Unneeded: Builtin `GLib Log Functions`
- ❌ void SetSaveFileDataCallback(SaveFileDataCallback callback); # Unneeded: Builtin `GLib Log Functions`
- ❌ void SetLoadFileTextCallback(LoadFileTextCallback callback); # Unneeded: Builtin `GLib Log Functions`
- ❌ void SetSaveFileTextCallback(SaveFileTextCallback callback); # Unneeded: Builtin `GLib Log Functions`
- ❌ unsigned char *LoadFileData(const char *fileName, int *dataSize); # Unneeded: Builtin `GLib File Functions`
- ❌ void UnloadFileData(unsigned char *data); # Unneeded: See above.
- ❌ bool SaveFileData(const char *fileName, void *data, int dataSize); # Unneeded: See above.
- ❌ bool ExportDataAsCode(const unsigned char *data, int dataSize, const char *fileName); # Unneeded: See above.
- ❌ char *LoadFileText(const char *fileName); # Unneeded: See above.
- ❌ void UnloadFileText(char *text); # Unneeded: See above.
- ❌ bool SaveFileText(const char *fileName, char *text); # Unneeded: See above.
- ❌ bool FileExists(const char *fileName); # Unneeded: See above.
- ❌ bool DirectoryExists(const char *dirPath); # Unneeded: See above.
- ❌ bool IsFileExtension(const char *fileName, const char *ext); # Unneeded: See above.
- ❌ int GetFileLength(const char *fileName); # Unneeded: See above.
- ❌ const char *GetFileExtension(const char *fileName); # Unneeded: See Above.
- ❌ const char *GetFileName(const char *filePath); # Unneeded: See Above.
- ❌ const char *GetFileNameWithoutExt(const char *filePath); # Unneeded: See Above.
- ❌ const char *GetDirectoryPath(const char *filePath); # Unneeded: See Above.
- ❌ const char *GetPrevDirectoryPath(const char *dirPath); # Unneeded: See Above.
- ❌ const char *GetWorkingDirectory(void); # Unneeded: Builtin `GLib.Environment.get_current_dir`
- ❌ const char *GetApplicationDirectory(void); # Unneeded: Builtin `GLib File Functions`
- ❌ bool ChangeDirectory(const char *dir); # Unneeded: Builtin `GLib.Environment.set_current_dir`
- ❌ bool IsPathFile(const char *path);
- ❌ FilePathList LoadDirectoryFiles(const char *dirPath); # Unneeded: Builtin `GLib.Dir`
- ❌ FilePathList LoadDirectoryFilesEx(const char *basePath, const char *filter, bool scanSubdirs); # Unneeded: Builtin `GLib.Dir`
- ❌ void UnloadDirectoryFiles(FilePathList files); # Unneeded: Builtin `GLib.Dir`
- [x] bool IsFileDropped(void); # Implemented: `Window.file_dropped`
- [x] FilePathList LoadDroppedFiles(void); # Implemented: `Window.get_dropped_files`
- [x] void UnloadDroppedFiles(FilePathList files); # Implemented: `Window.get_dropped_files`
- ❌ long GetFileModTime(const char *fileName); # Unneeded: Builtin `GLib.FileInfo.get_modification_date_time`
- ❌ unsigned char *CompressData(const unsigned char *data, int dataSize, int *compDataSize); # Unneeded: Built into GLib `GLib.ZlibCompressor`
- ❌ unsigned char *DecompressData(const unsigned char *compData, int compDataSize, int *dataSize); # Unneeded: Built into GLib `GLib.ZlibDecompressor`
- ❌ char *EncodeDataBase64(const unsigned char *data, int dataSize, int *outputSize); # Unneeded: Built into GLib. `GLib.Base64.encode`
- ❌ unsigned char *DecodeDataBase64(const unsigned char *data, int *outputSize); # Unneeded: Built into GLib. `GLib.Base64.decode`
- [x] AutomationEventList LoadAutomationEventList(const char *fileName); # Implemented: `Automation.EventList`
- [x] void UnloadAutomationEventList(AutomationEventList *list); # Implemented: `Automation.EventList`
- [x] bool ExportAutomationEventList(AutomationEventList list, const char *fileName); # Implemented: `Automation.EventList.export`
- [x] void SetAutomationEventList(AutomationEventList *list); # Implemented: `Automation.set_automation_event_list`
- [x] void SetAutomationEventBaseFrame(int frame); # Implemented: `Window.set_automation_event_base_frame`
- [x] void StartAutomationEventRecording(void); # Implemented: `Window.record_automation_events`
- [x] void StopAutomationEventRecording(void); # Implemented: `Window.record_automation_events`
- [x] void PlayAutomationEvent(AutomationEvent event); `Window.play_automation_event`
- [x] bool IsKeyPressed(int key); # Implemented: `Input.Keyboard.is_pressed`
- [x] bool IsKeyPressedRepeat(int key); # Implemented: `Input.Keyboard.is_pressed_repeat`
- [x] bool IsKeyDown(int key); # Implemented: `Input.Keyboard.is_down`
- [x] bool IsKeyReleased(int key); # Implemented: `Input.Keyboard.is_released`
- [x] bool IsKeyUp(int key); # Implemented: `Input.Keyboard.is_up`
- [x] int GetKeyPressed(void); # Implemented: `Input.Keyboard.key_pressed`
- [x] int GetCharPressed(void); # Implemented: `Input.Keyboard.char_pressed`
- [x] void SetExitKey(int key); # Implemented: `Window.exit_key`
- [x] bool IsGamepadAvailable(int gamepad); # Implemented: `Input.Gamepad.still_around`
- [x] const char *GetGamepadName(int gamepad); # Implemented `Input.Gamepad.name`
- [x] bool IsGamepadButtonPressed(int gamepad, int button); # Implemented: `Input.Gamepad.is_button_pressed`
- [x] bool IsGamepadButtonDown(int gamepad, int button); # Implemented: `Input.Gamepad.is_button_down`
- [x] bool IsGamepadButtonReleased(int gamepad, int button); # Implemented: `Input.Gamepad.is_button_released`
- [x] bool IsGamepadButtonUp(int gamepad, int button); # Implemented: `Input.Gamepad.is_button_up`
- [x] int GetGamepadButtonPressed(void); # Implemented: `Input.Gamepad.button_pressed`
- [x] int GetGamepadAxisCount(int gamepad); # Implemented: `Input.Gamepad.axis_count`
- [x] float GetGamepadAxisMovement(int gamepad, int axis); # Implemented: `Input.Gamepad.get_axis_movement`
- [x] int SetGamepadMappings(const char *mappings); # Implemented: `Input.Gamepad.set_mappings`
- [x] bool IsMouseButtonPressed(int button); # Implemented: `Input.Mouse.is_pressed`
- [x] bool IsMouseButtonDown(int button); # Implemented: `Input.Mouse.is_down`
- [x] bool IsMouseButtonReleased(int button); # Implemented: `Input.Mouse.is_released`
- [x] bool IsMouseButtonUp(int button); # Implemented: `Input.Mouse.is_up`
- [x] int GetMouseX(void); # Implemented: `Input.Mouse.x`
- [x] int GetMouseY(void); # Implemented: `Input.Mouse.y`
- [x] Vector2 GetMousePosition(void); # Implemented: `Input.Mouse.position`
- [x] Vector2 GetMouseDelta(void); # Implemented: `Input.Mouse.delta`
- [x] void SetMousePosition(int x, int y); # Implemented: `Input.Mouse.position`
- [x] void SetMouseOffset(int offsetX, int offsetY); # Implemented: `Input.Mouse.offset`
- [x] void SetMouseScale(float scaleX, float scaleY); # Implemented: `Input.Mouse.scale`
- [x] float GetMouseWheelMove(void); # Implemented: `Input.Mouse.wheel_move`
- [x] Vector2 GetMouseWheelMoveV(void); # Implemented: `Input.Mouse.wheel_move`
- [x] void SetMouseCursor(int cursor); # Implemented: `Input.Mouse.set_cursor`
- [x] int GetTouchX(void); # Implemented: `Input.Touch.x`
- [x] int GetTouchY(void); # Implemented: `Input.Touch.y`
- [x] Vector2 GetTouchPosition(int index); # Implemented: `Input.Touch.get_position`
- [x] int GetTouchPointId(int index); # Implemented: `Input.Touch.get_id`
- [x] int GetTouchPointCount(void); # Implemented: `Input.Touch.point_count`
- [x] void SetGesturesEnabled(unsigned int flags); # Implemented: `Input.Touch.enable_gestures`
- [x] bool IsGestureDetected(unsigned int gesture); # Implemented: `Input.Touch.is_gesture_detected`
- [x] int GetGestureDetected(void); # Implemented: `Input.Touch.detected_gesture`
- [x] float GetGestureHoldDuration(void); # Implemented: `Input.Touch.hold_duration`
- [x] Vector2 GetGestureDragVector(void); # Implemented: `Input.Touch.drag_vector`
- [x] float GetGestureDragAngle(void); # Implemented: `Input.Touch.drag_angle`
- [x] Vector2 GetGesturePinchVector(void); # Implemented: `Input.Touch.pinch_vector`
- [x] float GetGesturePinchAngle(void); # Implemented: `Input.Touch.pinch_angle`
- [ ] void UpdateCamera(Camera *camera, int mode);
- [ ] void UpdateCameraPro(Camera *camera, Vector3 movement, Vector3 rotation, float zoom);

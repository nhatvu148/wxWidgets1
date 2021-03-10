# Note on ANSI vs UNICODE:

- If you are compiling in ANSI (MBCS), use \_T(""). This will allow you to transition to UNICODE with the minimum amount of trouble.
- If you are compiling in UNICODE (and never need to compile in ANSI), use L"".

# Precompiled headers:

- stdafx.h
- pch.h
- Simply list all your big huge headers for your APIs in your stdafx.h file, in the appropriate order, and then start each of your CPP files at the very top with an #include "stdafx.h", before any meaningful content.

# Build from source:

- "C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\MSBuild\Current\Bin\MSBuild.exe"
- msbuild myproject.vcxproj /p:configuration=debug /p:platform=win32

# WXWIDGETS:

- https://www.wxwidgets.org/docs/tutorials/
- https://www.wxwidgets.org/downloads/
- https://www.youtube.com/watch?v=sRhoZcNpMb4

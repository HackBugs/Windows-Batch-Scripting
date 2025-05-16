# Save this file with bat file like example - example.bat

```
@echo off
color 0A
title AI Tools & Research Launcher
cls

:menu
echo ===================================================
echo         AI TOOLS & RESEARCH LAUNCHER
echo ===================================================
echo.
echo  [1] AI Chat Assistants
echo  [2] Coding Tools
echo  [3] Stock Market & Trading Research
echo  [4] Technology News & Trends
echo  [5] All Groups (Separate Windows)
echo  [6] All Groups (With Browser Grouping)
echo  [0] Exit
echo.
echo ===================================================

set /p choice="Enter your choice (0-6): "

if "%choice%"=="0" goto exit
if "%choice%"=="1" goto ai_chats
if "%choice%"=="2" goto coding_tools
if "%choice%"=="3" goto stock_market
if "%choice%"=="4" goto tech_news
if "%choice%"=="5" goto all_groups
if "%choice%"=="6" goto all_groups_with_grouping
echo Invalid choice. Please try again.
timeout /t 2 >nul
cls
goto menu

:ai_chats
cls
echo ===================================================
echo          OPENING AI CHAT ASSISTANTS
echo ===================================================
echo.
echo  • ChatGPT
echo  • Google Gemini
echo  • Claude AI
echo  • Poe (Llama 3)
echo  • DeepSeek
echo  • Perplexity
echo  • Hugging Face Chat
echo  • Pi.ai
echo  • Character.AI
echo.

REM Path to Microsoft Edge - update if needed
set "EDGE_PATH=C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe"

start "" "%EDGE_PATH%" --new-window ^
    "https://chat.openai.com/" ^
    "https://gemini.google.com/" ^
    "https://claude.ai/" ^
    "https://poe.com/Meta-Llama-3-70b-chat" ^
    "https://chat.deepseek.com/" ^
    "https://www.perplexity.ai/" ^
    "https://huggingface.co/chat/" ^
    "https://pi.ai/" ^
    "https://beta.character.ai/"

echo Done! AI Chat Assistants window opened.
echo.
pause
cls
goto menu

:coding_tools
cls
echo ===================================================
echo             OPENING CODING TOOLS
echo ===================================================
echo.
echo  • Cursor
echo  • v0.dev
echo  • GitHub Copilot
echo  • Replit
echo  • CodeSandbox
echo  • CodePen
echo  • StackBlitz
echo  • Figma AI
echo  • Codeium
echo.

set "EDGE_PATH=C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe"

start "" "%EDGE_PATH%" --new-window ^
    "https://cursor.sh/" ^
    "https://v0.dev/" ^
    "https://github.com/features/copilot" ^
    "https://replit.com/" ^
    "https://codesandbox.io/" ^
    "https://codepen.io/" ^
    "https://stackblitz.com/" ^
    "https://www.figma.com/ai" ^
    "https://codeium.com/"

echo Done! Coding Tools window opened.
echo.
pause
cls
goto menu

:stock_market
cls
echo ===================================================
echo      OPENING STOCK MARKET & TRADING RESEARCH
echo ===================================================
echo.
echo  • Yahoo Finance
echo  • TradingView
echo  • Bloomberg Markets
echo  • MarketWatch
echo  • Investing.com
echo  • Seeking Alpha
echo  • Finviz
echo  • Morningstar
echo  • Koyfin
echo.

set "EDGE_PATH=C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe"

start "" "%EDGE_PATH%" --new-window ^
    "https://finance.yahoo.com/" ^
    "https://www.tradingview.com/" ^
    "https://www.bloomberg.com/markets" ^
    "https://www.marketwatch.com/" ^
    "https://www.investing.com/" ^
    "https://seekingalpha.com/" ^
    "https://finviz.com/" ^
    "https://www.morningstar.com/" ^
    "https://www.koyfin.com/"

echo Done! Stock Market & Trading Research window opened.
echo.
pause
cls
goto menu

:tech_news
cls
echo ===================================================
echo        OPENING TECHNOLOGY NEWS & TRENDS
echo ===================================================
echo.
echo  • Ars Technica
echo  • The Verge
echo  • TechCrunch
echo  • Wired
echo  • MIT Technology Review
echo  • Protocol
echo  • Axios Technology
echo  • Reuters Technology
echo  • Hacker News
echo.

set "EDGE_PATH=C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe"

start "" "%EDGE_PATH%" --new-window ^
    "https://arstechnica.com/" ^
    "https://www.theverge.com/" ^
    "https://techcrunch.com/" ^
    "https://www.wired.com/" ^
    "https://www.technologyreview.com/" ^
    "https://www.protocol.com/" ^
    "https://www.axios.com/technology" ^
    "https://www.reuters.com/technology/" ^
    "https://news.ycombinator.com/"

echo Done! Technology News & Trends window opened.
echo.
pause
cls
goto menu

:all_groups
cls
echo ===================================================
echo      OPENING ALL GROUPS IN SEPARATE WINDOWS
echo ===================================================
echo.
echo  • Opening AI Chat Assistants...
call :ai_chats_silent
echo  • Opening Coding Tools...
call :coding_tools_silent
echo  • Opening Stock Market & Trading Research...
call :stock_market_silent
echo  • Opening Technology News & Trends...
call :tech_news_silent
echo.
echo Done! All groups opened in separate windows.
echo.
pause
cls
goto menu

:all_groups_with_grouping
cls
echo ===================================================
echo      OPENING ALL GROUPS WITH BROWSER GROUPING
echo ===================================================
echo.
echo This will open all sites and you'll need to manually
echo organize them into groups in Edge using:
echo.
echo  1. Right-click on a tab
echo  2. Select "Add all tabs to a new group"
echo  3. Name and color-code each group
echo.
echo  • Opening AI Chat Assistants...
set "EDGE_PATH=C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe"

start "" "%EDGE_PATH%" --new-window ^
    "https://chat.openai.com/" ^
    "https://gemini.google.com/" ^
    "https://claude.ai/" ^
    "https://poe.com/Meta-Llama-3-70b-chat" ^
    "https://chat.deepseek.com/" ^
    "https://www.perplexity.ai/" ^
    "https://huggingface.co/chat/" ^
    "https://pi.ai/" ^
    "https://beta.character.ai/" ^
    "https://cursor.sh/" ^
    "https://v0.dev/" ^
    "https://github.com/features/copilot" ^
    "https://replit.com/" ^
    "https://codesandbox.io/" ^
    "https://codepen.io/" ^
    "https://stackblitz.com/" ^
    "https://www.figma.com/ai" ^
    "https://codeium.com/" ^
    "https://finance.yahoo.com/" ^
    "https://www.tradingview.com/" ^
    "https://www.bloomberg.com/markets" ^
    "https://www.marketwatch.com/" ^
    "https://www.investing.com/" ^
    "https://seekingalpha.com/" ^
    "https://finviz.com/" ^
    "https://www.morningstar.com/" ^
    "https://www.koyfin.com/" ^
    "https://arstechnica.com/" ^
    "https://www.theverge.com/" ^
    "https://techcrunch.com/" ^
    "https://www.wired.com/" ^
    "https://www.technologyreview.com/" ^
    "https://www.protocol.com/" ^
    "https://www.axios.com/technology" ^
    "https://www.reuters.com/technology/" ^
    "https://news.ycombinator.com/"

echo.
echo Done! All sites opened in one window.
echo Please organize them into tab groups manually.
echo.
pause
cls
goto menu

:ai_chats_silent
set "EDGE_PATH=C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe"
start "" "%EDGE_PATH%" --new-window ^
    "https://chat.openai.com/" ^
    "https://gemini.google.com/" ^
    "https://claude.ai/" ^
    "https://poe.com/Meta-Llama-3-70b-chat" ^
    "https://chat.deepseek.com/" ^
    "https://www.perplexity.ai/" ^
    "https://huggingface.co/chat/" ^
    "https://pi.ai/" ^
    "https://beta.character.ai/"
timeout /t 2 >nul
exit /b

:coding_tools_silent
set "EDGE_PATH=C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe"
start "" "%EDGE_PATH%" --new-window ^
    "https://cursor.sh/" ^
    "https://v0.dev/" ^
    "https://github.com/features/copilot" ^
    "https://replit.com/" ^
    "https://codesandbox.io/" ^
    "https://codepen.io/" ^
    "https://stackblitz.com/" ^
    "https://www.figma.com/ai" ^
    "https://codeium.com/"
timeout /t 2 >nul
exit /b

:stock_market_silent
set "EDGE_PATH=C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe"
start "" "%EDGE_PATH%" --new-window ^
    "https://finance.yahoo.com/" ^
    "https://www.tradingview.com/" ^
    "https://www.bloomberg.com/markets" ^
    "https://www.marketwatch.com/" ^
    "https://www.investing.com/" ^
    "https://seekingalpha.com/" ^
    "https://finviz.com/" ^
    "https://www.morningstar.com/" ^
    "https://www.koyfin.com/"
timeout /t 2 >nul
exit /b

:tech_news_silent
set "EDGE_PATH=C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe"
start "" "%EDGE_PATH%" --new-window ^
    "https://arstechnica.com/" ^
    "https://www.theverge.com/" ^
    "https://techcrunch.com/" ^
    "https://www.wired.com/" ^
    "https://www.technologyreview.com/" ^
    "https://www.protocol.com/" ^
    "https://www.axios.com/technology" ^
    "https://www.reuters.com/technology/" ^
    "https://news.ycombinator.com/"
timeout /t 2 >nul
exit /b

:exit
cls
echo ===================================================
echo                THANK YOU FOR USING
echo           AI TOOLS & RESEARCH LAUNCHER
echo ===================================================
echo.
timeout /t 3 >nul
exit
```

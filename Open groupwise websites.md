```
@echo off
chcp 1252 >nul
color 0A
title AI Tools and Research Launcher
cls

:menu
echo ===================================================
echo         AI TOOLS AND RESEARCH LAUNCHER
echo ===================================================
echo.
echo  [1] AI Chat Assistants
echo  [2] Coding Tools
echo  [3] Stock Market and Trading Research
echo  [4] Technology News and Trends
echo  [5] All Groups (Separate Windows)
echo  [6] All Groups (With Browser Grouping)
echo  [0] Exit
echo.
echo ===================================================
echo.

set /p choice="Enter your choice (0-6): "

if "%choice%"=="0" goto exit
if "%choice%"=="1" goto ai_chats_menu
if "%choice%"=="2" goto coding_tools_menu
if "%choice%"=="3" goto stock_market_menu
if "%choice%"=="4" goto tech_news_menu
if "%choice%"=="5" goto all_groups
if "%choice%"=="6" goto all_groups_with_grouping
echo Invalid choice. Please try again.
timeout /t 2 >nul
cls
goto menu

:ai_chats_menu
cls
echo ===================================================
echo          AI CHAT ASSISTANTS - SELECT OPTION
echo ===================================================
echo.
echo  [1] Open All AI Chat Assistants
echo.
echo  [2] ChatGPT
echo  [3] Google Gemini
echo  [4] Claude AI
echo  [5] Poe (Llama 3)
echo  [6] DeepSeek
echo  [7] Perplexity
echo  [8] Hugging Face Chat
echo  [9] Pi.ai
echo [10] Character.AI
echo.
echo  [0] Back to Main Menu
echo.
echo ===================================================
echo.

set /p ai_choice="Enter your choice (0-10): "

if "%ai_choice%"=="0" goto menu
if "%ai_choice%"=="1" goto ai_chats_all
if "%ai_choice%"=="2" goto open_chatgpt
if "%ai_choice%"=="3" goto open_gemini
if "%ai_choice%"=="4" goto open_claude
if "%ai_choice%"=="5" goto open_poe
if "%ai_choice%"=="6" goto open_deepseek
if "%ai_choice%"=="7" goto open_perplexity
if "%ai_choice%"=="8" goto open_huggingface
if "%ai_choice%"=="9" goto open_piai
if "%ai_choice%"=="10" goto open_characterai
echo Invalid choice. Please try again.
timeout /t 2 >nul
goto ai_chats_menu

:ai_chats_all
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
echo Opened all AI Chat Assistants
timeout /t 2 >nul
goto ai_chats_menu

:open_chatgpt
start "" "https://chat.openai.com/"
echo Opened ChatGPT
timeout /t 2 >nul
goto ai_chats_menu

:open_gemini
start "" "https://gemini.google.com/"
echo Opened Google Gemini
timeout /t 2 >nul
goto ai_chats_menu

:open_claude
start "" "https://claude.ai/"
echo Opened Claude AI
timeout /t 2 >nul
goto ai_chats_menu

:open_poe
start "" "https://poe.com/Meta-Llama-3-70b-chat"
echo Opened Poe (Llama 3)
timeout /t 2 >nul
goto ai_chats_menu

:open_deepseek
start "" "https://chat.deepseek.com/"
echo Opened DeepSeek
timeout /t 2 >nul
goto ai_chats_menu

:open_perplexity
start "" "https://www.perplexity.ai/"
echo Opened Perplexity
timeout /t 2 >nul
goto ai_chats_menu

:open_huggingface
start "" "https://huggingface.co/chat/"
echo Opened Hugging Face Chat
timeout /t 2 >nul
goto ai_chats_menu

:open_piai
start "" "https://pi.ai/"
echo Opened Pi.ai
timeout /t 2 >nul
goto ai_chats_menu

:open_characterai
start "" "https://beta.character.ai/"
echo Opened Character.AI
timeout /t 2 >nul
goto ai_chats_menu

:coding_tools_menu
cls
echo ===================================================
echo             CODING TOOLS - SELECT OPTION
echo ===================================================
echo.
echo  [1] Open All Coding Tools
echo.
echo  [2] Cursor
echo  [3] v0.dev
echo  [4] GitHub Copilot
echo  [5] Replit
echo  [6] CodeSandbox
echo  [7] CodePen
echo  [8] StackBlitz
echo  [9] Figma AI
echo [10] Codeium
echo.
echo  [0] Back to Main Menu
echo.
echo ===================================================
echo.

set /p code_choice="Enter your choice (0-10): "

if "%code_choice%"=="0" goto menu
if "%code_choice%"=="1" goto coding_tools_all
if "%code_choice%"=="2" goto open_cursor
if "%code_choice%"=="3" goto open_v0dev
if "%code_choice%"=="4" goto open_copilot
if "%code_choice%"=="5" goto open_replit
if "%code_choice%"=="6" goto open_codesandbox
if "%code_choice%"=="7" goto open_codepen
if "%code_choice%"=="8" goto open_stackblitz
if "%code_choice%"=="9" goto open_figmaai
if "%code_choice%"=="10" goto open_codeium
echo Invalid choice. Please try again.
timeout /t 2 >nul
goto coding_tools_menu

:coding_tools_all
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
echo Opened all Coding Tools
timeout /t 2 >nul
goto coding_tools_menu

:open_cursor
start "" "https://cursor.sh/"
echo Opened Cursor
timeout /t 2 >nul
goto coding_tools_menu

:open_v0dev
start "" "https://v0.dev/"
echo Opened v0.dev
timeout /t 2 >nul
goto coding_tools_menu

:open_copilot
start "" "https://github.com/features/copilot"
echo Opened GitHub Copilot
timeout /t 2 >nul
goto coding_tools_menu

:open_replit
start "" "https://replit.com/"
echo Opened Replit
timeout /t 2 >nul
goto coding_tools_menu

:open_codesandbox
start "" "https://codesandbox.io/"
echo Opened CodeSandbox
timeout /t 2 >nul
goto coding_tools_menu

:open_codepen
start "" "https://codepen.io/"
echo Opened CodePen
timeout /t 2 >nul
goto coding_tools_menu

:open_stackblitz
start "" "https://stackblitz.com/"
echo Opened StackBlitz
timeout /t 2 >nul
goto coding_tools_menu

:open_figmaai
start "" "https://www.figma.com/ai"
echo Opened Figma AI
timeout /t 2 >nul
goto coding_tools_menu

:open_codeium
start "" "https://codeium.com/"
echo Opened Codeium
timeout /t 2 >nul
goto coding_tools_menu

:stock_market_menu
cls
echo ===================================================
echo      STOCK MARKET AND TRADING - SELECT OPTION
echo ===================================================
echo.
echo  [1] Open All Stock Market Tools
echo.
echo  [2] Yahoo Finance
echo  [3] TradingView
echo  [4] Bloomberg Markets
echo  [5] MarketWatch
echo  [6] Investing.com
echo  [7] Seeking Alpha
echo  [8] Finviz
echo  [9] Morningstar
echo [10] Koyfin
echo.
echo  [0] Back to Main Menu
echo.
echo ===================================================
echo.

set /p stock_choice="Enter your choice (0-10): "

if "%stock_choice%"=="0" goto menu
if "%stock_choice%"=="1" goto stock_market_all
if "%stock_choice%"=="2" goto open_yahoo
if "%stock_choice%"=="3" goto open_tradingview
if "%stock_choice%"=="4" goto open_bloomberg
if "%stock_choice%"=="5" goto open_marketwatch
if "%stock_choice%"=="6" goto open_investing
if "%stock_choice%"=="7" goto open_seekingalpha
if "%stock_choice%"=="8" goto open_finviz
if "%stock_choice%"=="9" goto open_morningstar
if "%stock_choice%"=="10" goto open_koyfin
echo Invalid choice. Please try again.
timeout /t 2 >nul
goto stock_market_menu

:stock_market_all
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
echo Opened all Stock Market Tools
timeout /t 2 >nul
goto stock_market_menu

:open_yahoo
start "" "https://finance.yahoo.com/"
echo Opened Yahoo Finance
timeout /t 2 >nul
goto stock_market_menu

:open_tradingview
start "" "https://www.tradingview.com/"
echo Opened TradingView
timeout /t 2 >nul
goto stock_market_menu

:open_bloomberg
start "" "https://www.bloomberg.com/markets"
echo Opened Bloomberg Markets
timeout /t 2 >nul
goto stock_market_menu

:open_marketwatch
start "" "https://www.marketwatch.com/"
echo Opened MarketWatch
timeout /t 2 >nul
goto stock_market_menu

:open_investing
start "" "https://www.investing.com/"
echo Opened Investing.com
timeout /t 2 >nul
goto stock_market_menu

:open_seekingalpha
start "" "https://seekingalpha.com/"
echo Opened Seeking Alpha
timeout /t 2 >nul
goto stock_market_menu

:open_finviz
start "" "https://finviz.com/"
echo Opened Finviz
timeout /t 2 >nul
goto stock_market_menu

:open_morningstar
start "" "https://www.morningstar.com/"
echo Opened Morningstar
timeout /t 2 >nul
goto stock_market_menu

:open_koyfin
start "" "https://www.koyfin.com/"
echo Opened Koyfin
timeout /t 2 >nul
goto stock_market_menu

:tech_news_menu
cls
echo ===================================================
echo        TECHNOLOGY NEWS AND TRENDS - SELECT OPTION
echo ===================================================
echo.
echo  [1] Open All Tech News Sites
echo.
echo  [2] Ars Technica
echo  [3] The Verge
echo  [4] TechCrunch
echo  [5] Wired
echo  [6] MIT Technology Review
echo  [7] Protocol
echo  [8] Axios Technology
echo  [9] Reuters Technology
echo [10] Hacker News
echo.
echo  [0] Back to Main Menu
echo.
echo ===================================================
echo.

set /p tech_choice="Enter your choice (0-10): "

if "%tech_choice%"=="0" goto menu
if "%tech_choice%"=="1" goto tech_news_all
if "%tech_choice%"=="2" goto open_arstechnica
if "%tech_choice%"=="3" goto open_theverge
if "%tech_choice%"=="4" goto open_techcrunch
if "%tech_choice%"=="5" goto open_wired
if "%tech_choice%"=="6" goto open_mittech
if "%tech_choice%"=="7" goto open_protocol
if "%tech_choice%"=="8" goto open_axios
if "%tech_choice%"=="9" goto open_reuters
if "%tech_choice%"=="10" goto open_hackernews
echo Invalid choice. Please try again.
timeout /t 2 >nul
goto tech_news_menu

:tech_news_all
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
echo Opened all Technology News Sites
timeout /t 2 >nul
goto tech_news_menu

:open_arstechnica
start "" "https://arstechnica.com/"
echo Opened Ars Technica
timeout /t 2 >nul
goto tech_news_menu

:open_theverge
start "" "https://www.theverge.com/"
echo Opened The Verge
timeout /t 2 >nul
goto tech_news_menu

:open_techcrunch
start "" "https://techcrunch.com/"
echo Opened TechCrunch
timeout /t 2 >nul
goto tech_news_menu

:open_wired
start "" "https://www.wired.com/"
echo Opened Wired
timeout /t 2 >nul
goto tech_news_menu

:open_mittech
start "" "https://www.technologyreview.com/"
echo Opened MIT Technology Review
timeout /t 2 >nul
goto tech_news_menu

:open_protocol
start "" "https://www.protocol.com/"
echo Opened Protocol
timeout /t 2 >nul
goto tech_news_menu

:open_axios
start "" "https://www.axios.com/technology"
echo Opened Axios Technology
timeout /t 2 >nul
goto tech_news_menu

:open_reuters
start "" "https://www.reuters.com/technology/"
echo Opened Reuters Technology
timeout /t 2 >nul
goto tech_news_menu

:open_hackernews
start "" "https://news.ycombinator.com/"
echo Opened Hacker News
timeout /t 2 >nul
goto tech_news_menu

:all_groups
cls
echo ===================================================
echo      OPENING ALL GROUPS IN SEPARATE WINDOWS
echo ===================================================
echo.
echo   - Opening AI Chat Assistants...
call :ai_chats_silent
echo   - Opening Coding Tools...
call :coding_tools_silent
echo   - Opening Stock Market and Trading Research...
call :stock_market_silent
echo   - Opening Technology News and Trends...
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
echo   - Opening all sites in one window...

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
echo           AI TOOLS AND RESEARCH LAUNCHER
echo ===================================================
echo.
timeout /t 3 >nul
exit
```

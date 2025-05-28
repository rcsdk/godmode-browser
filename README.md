# godmode-browser


Information about the browser and possible solutions;


https://github.com/smol-ai/GodMode

https://github.com/smol-ai/GodMode/releases/tag/v1.0.0-beta.10

https://github.com/smol-ai/GodMode/tree/main/scripts

https://github.com/smol-ai/GodMode/tree/main/assets   ----icons





Overview of Smol AI and GodMode Browser
GodMode is a specialized chat browser developed by the smol-ai project designed to facilitate quick and simultaneous access to multiple AI web applications such as ChatGPT, Claude 2, Perplexity, Bing, and others through a single interface and keyboard shortcut (Cmd+Shift+G). It essentially embeds these web apps as webviews, letting users type once and send input to all or select apps independently.

This browser is lightweight, focused solely on AI chat webapps, and available for macOS (Apple Silicon and Intel), with Windows and Linux support in early stages needing further development.

About Smol AI
The smol-ai ecosystem includes several AI tools and libraries:

GodMode Browser: Dedicated AI chat browser as above.

Smol AI Developer: A library that acts like a junior AI developer, transforming product specs into codebases, enabling embedding AI development capabilities in apps.

Smol Agents: Lightweight autonomous AI agents designed to run locally in browsers or terminals with minimal resources, capable of performing tasks autonomously by interacting with APIs, tools, or software. These agents emphasize simplicity, transparency, and hackability, suitable for local use without heavy cloud dependencies.

Your Issue: White Screen on Kali Linux KDE X11 with GodMode
You report that when using GodMode on Kali Linux with KDE on X11, clicking any link or button (such as ChatGPT or Claude) causes the screen to go white except for a thin top menu bar.

Possible Causes and Suggestions
Browser/Webview Rendering Issues on Linux KDE X11: GodMode uses webviews to embed AI webapps. On Linux, especially with KDE and X11, webview rendering can sometimes be unstable or incompatible due to GPU acceleration, compositing, or library dependencies.

Incomplete or Experimental Linux Support: The GodMode project notes that Windows/Linux support is recent and "needs a lot of work" with calls for help, indicating the Linux version may be unstable or have unresolved bugs.

Authentication or Session Issues: Some AI webapps like Google Bard have complex auth requirements that may cause loading failures or white screens if not properly logged in or if cookies/sessions are not handled correctly.

Extensions or Environment Conflicts: Similar to browser issues described for ChatGPT dropdown problems in Chrome/Edge (where extensions or cache cause UI failures), your environment might have conflicts affecting the embedded webviews.

Troubleshooting Steps
Check for Updates: Ensure you have the latest GodMode Linux build or consider building from source to get recent fixes.

Try Disabling GPU Acceleration: Run GodMode with GPU acceleration disabled or use environment variables to force software rendering to see if rendering issues resolve.

Test on Different Desktop Environments or Wayland: If possible, try running GodMode on a different DE or under Wayland instead of X11 to isolate compositor-related issues.

Clear Cache and Cookies: If GodMode stores session data, try clearing it or re-logging in.

Check Logs: Run GodMode from a terminal to capture error messages which may indicate missing dependencies or rendering errors.

Use Alternative Browsers: As a fallback, use Firefox or Chrome directly for accessing these AI webapps until Linux support matures.

Summary
GodMode is a smol-ai project chat browser focused on AI webapps, currently experimental on Linux with known instability.

Smol Agents and Smol AI Developer are related AI tools for local autonomous agents and AI-assisted development, respectively.

Your white screen issue on Kali KDE X11 likely stems from incomplete Linux support or rendering incompatibilities in GodMode's webviews.

Try troubleshooting with GPU settings, environment changes, or logs, and consider using mainstream browsers as a temporary alternative.

If you are compiling a GitHub repository or documentation, these points and references provide a comprehensive overview of the smol-ai ecosystem and known limitations of GodMode on Linux.







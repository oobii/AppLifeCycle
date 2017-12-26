# AppLifeCycle
The AppDelegate class conforms to the UIApplicationDelegate protocol, which defines methods that serve as hooks into the different events in the app's life cycle

#### Run the app in Simulator. When you open the app, you'll see two messages print to the console:
- Did finish launching.
- Did become active.
      
#### Press Shift-Command-H to simulate pressing the Home button and dismissing the app. You'll see two more messages print to the console:
- Will resign active.
- Did enter background.
      
#### Open the app switcher by pressing Shift-Command-H two times, and reopen the app. You'll see another two messages print to the console:
- Will enter foreground.
- Did become active.
      
#### Open the app switcher again, then return to the app.
 - Will resign active.
 - Did become active.


For apps that are allowed to execute code in the background—such as apps that provide GPS directions, play music, or handle audio calls—you'll want to call the **applicationDidEnterBackground** function. For apps that don't normally run in the background, you'll use the applicationWillTerminate function.



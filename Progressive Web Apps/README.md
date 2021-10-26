<img src="https://web-dev.imgix.net/image/tcFciHGuF3MxnTr1y5ue01OGLBn2/LvIq0sbMK73ycjb2yomw.svg" width="200" alt="Progressive Web Apps" title="Progressive Web Apps">

# Progressive Web Apps

## What is Progressive Web Apps

The web is an incredible platform. Its mix of ubiquity across devices and operating systems, its user-centered security model, and the fact that neither its specification nor its implementation is controlled by a single company makes the web a unique platform to develop software on. Combined with its inherent linkability, it's possible to search it and share what you've found with anyone, anywhere. Whenever you go to a website, it's up-to-date, and your experience with that site can be as ephemeral or as permanent as you'd like. Web applications can reach anyone, anywhere, on any device with a single codebase.

Platform-specific applications, are known for being incredibly rich and reliable. They're ever-present, on home screens, docks, and taskbars. They work regardless of network connection. They launch in their own standalone experience. They can read and write files from the local file system, access hardware connected via USB, serial or bluetooth, and even interact with data stored on your device, like contacts and calendar events. In these applications, you can do things like take pictures, see playing songs listed on the home screen, or control song playback while in another app. Platform-specific applications feel like part of the device they run on.

If you think about platform-specific apps and web apps in terms of capabilities and reach, platform-specific apps represent the best of capabilities whereas web apps represent the best of reach. So where do Progressive Web Apps fit in?

Progressive Web Apps (PWA) are built and enhanced with modern APIs to deliver enhanced capabilities, reliability, and installability while reaching anyone, anywhere, on any device with a single codebase.

The three app pillars #
Progressive Web Apps are web applications that have been designed so they are capable, reliable, and installable. These three pillars transform them into an experience that feels like a platform-specific application.

Capable #
The web is quite capable in its own right today. For example, you can build a hyper-local video chat app using WebRTC, geolocation, and push notifications. You can make that app installable and take those conversations virtual with WebGL and WebVR. With the introduction of WebAssembly, developers can tap into other ecosystems, like C, C++, and Rust, and bring decades of work and capabilities to the web too. Squoosh.app, for instance, leverages this for its advanced image compression.

Until recently, only platform-specific apps could really lay claim to these capabilities. While some capabilities are still out of the web's reach, new and upcoming APIs are looking to change that, expanding what the web can do with features like file system access, media controls, app badging, and full clipboard support. All of these capabilities are built with the web's secure, user-centric permission model, ensuring that going to a website is never a scary proposition for users.

Between modern APIs, WebAssembly, and new and upcoming APIs, web applications are more capable than ever, and those capabilities are only growing.

## What does it take to be installable?

Progressive Web Apps (PWAs) are modern, high quality applications built using web technology. PWAs offer similar capabilities to iOS/Android/desktop apps, they are reliable even in unstable network conditions, and are installable making it easier for users to find and use them.

Most users are familiar with installing applications, and the benefits of an installed experience. Installed applications appear on operating system launch surfaces, such as the Applications folder on Mac OS X, the Start menu on Windows, and the homescreen on Android and iOS. Installed applications also show up in the activity switcher, device search engines such as Spotlight and in content sharing sheets.

Most browsers indicate to the user that your Progressive Web App (PWA) is installable when it meets certain criteria. Example indicators include an Install button in the address bar, or an Install menu item in the overflow menu.

In addition, when the criteria is met, many browsers will fire a beforeinstallprompt event, allowing you to provide a custom in-app UX that that will trigger the install flow within your app.

Install criteria #
In Chrome, your Progressive Web App must meet the following criteria before it will fire the beforeinstallprompt event and show the in-browser install promotion:

The web app is not already installed
Meets a user engagement heuristic
Be served over HTTPS
Includes a <a href="https://web.dev/add-manifest/">web app manifest </a> that includes:
short_name or name
icons - must include a 192px and a 512px icon
start_url
display - must be one of fullscreen, standalone, or minimal-ui
prefer_related_applications must not be present, or be false
Registers a service worker with a fetch handler
Other browsers have similar criteria for installation, though there may be minor differences. Check the respective sites for full details:

Edge
Firefox
Opera
Samsung Internet
UC Browser
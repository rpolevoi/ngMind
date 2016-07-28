# ngMind="beginner.mind"

A __progressive course__ of 26 __ANGULAR 2__ plunker demos to master core integrated concepts before writing a word of code.

Complete list of demo-links is at the bottom of this doc.

(You can jump to first demo here below, but *please* try reading this Intro doc first -- it's well worth the time):

[**Plunker Demo #1**](http://plnkr.co/edit/4A4juKPbXMrWzObNNal1?p=info)
-- SIMPLEST POSSIBLE COMPONENT (NON-DYNAMIC)
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo1)

###INTRO

The title of these demos honors Shenryu Suzuki's "Zen Mind, Beginner Mind," where the author made a famous observation. *“In the beginner’s mind"* he said, *"there are many possibilities, but in the expert’s there are few.”*

 Angular 2 is revolutionary, but the experienced developer cannot help but filter it through pre-existing constructs. It is therefore best approached with the most spacious possible mentality, and a certain deliberate humbleness.

###WHY LEARN ANGULAR 2?

Angular 2 is heavy lifting for anyone, however ponderous their cerebral cortex. In fact, at the start it can feel like climbing a wall of ice. Thus it's fair to ask why one should take the time and risk to study it with the intensity that it demands. If the answer here seems lengthy, consider the importance of the question.

Angular 2 is a __very big thing__. Bigger than Angular 1, bigger than Rails, bigger than React. No mere framework, but a __platform__. This means that Angular 2 must be compared to the Windows operating system or, more accurately, to Java, as creating a fundamental technological foundation for new kinds of development, with a potential lifespan measured in decades. Like both Windows and Java, the association with a dominant tech enterprise is crucial. It's simply impossible that Google will fail to support and press forward with the Angular project, long past version 2. And its motives for doing so are more powerful than mere *noblesse oblige* or good developer relations.

Microsoft had an enormous stake in the success of Windows development because sales of the operating system was its bread and butter. Sun had an important stake in Java because it believed that a continuing market for its high-priced servers depended on its prescient vision of a future __internet of applications__. And Java was both a first-class programming language and a technology (the Java Virtual Machine) that bridged across operating systems. The comparison to Angular 2 is obvious. Its language may be, strictly speaking, JavaScript (although written in TypeScript), but there is so much intellectual and syntactic superstructure that the underlying JS ends up buried under uniquely Angular code and thought patterns. The technology is the browser. But no one understands the browser and JavaScript interpretation the way that Google does, and the bottom line is transparently connecting JavaScript code to the browser DOM in a way that really works. When an Angular developer binds a JavaScript property to a DOM property, he or she can feel confident that the latter will always reflect the value of the former, and that this convenience (which inherently involves a great deal of under-the-hood complexity) will come at negligible cost to performance.

But Angular 2 is also Google's attempt to shape and anticipate the future scale and possibilities of __web development as true application development__, just as Sun's vision was with Java. This goal accounts for almost all that is new, difficult, or even revolutionary in Angular 2. And, just as with Java, there is a serious business strategy here. Google is taking aim at what, for it (and possibly for all of us) was the __great disaster of mobile development__. This was the decision driven by Steve Jobs and Apple as the first dominant force in mobile, that the mobile experience would live within locally-installed applications downloaded from a “store” over which the company had exclusive control. Jobs expected people to pay for their apps for the most part, and for Apple to share in this revenue just as it shared in music downloads.

There was, certainly at first, a valid technological argument supporting this, because short battery life, limited memory and processing power, and weak and expensive wireless service all converged to argue for downloading and installing an app only once for any given version, and loading it from local memory, only tapping data access from the internet as needed. Against this background, Google could do nothing more than launch a competing OS to prevent Apple from owning mobile completely, but this strategy never made sense for the company's crown jewel -- web search -- because mobile apps, living outside the browser were not searchable. With a flood of new apps appearing every day, the need for simple, universal Google search to provide them with visibility is glaringly obvious.

The answer is to replace the native or hybrid mobile app as we know it, and replace it with what Google calls the __"progressive web app__." This model for development, which works right now in primitive examples, involves matching the user experience of native mobile apps in a __web app living in the browser__. Instant loading of at least the initial interface from browser storage. Offline capabilities, especially during wireless service interruptions. The appearance of a dedicated app, with browser features hidden unless sought. And most importantly, the killer feature mobile apps cannot pretend to offer: __deep-linking of urls assigned to application state views__. A user can copy an url, even from deep within the app, and send it in an email as a link, where it can move to social media or web sites. And Google can find such links and make them searchable. That this is critical for Google is obvious. But it is also good for all of us who understand how hard it is to launch new mobile apps in such a crowded universe without the help of Google Search.

Should you doubt if this is really the most salient motive for Google with Angular 2 -- as the __ideal platform for displacing native mobile apps with searchable web apps the run everywhere__ -- check out the primary position given to progressive web apps on the Angular website Features page. In fact, Google goes much further, stressing that Angular is a clear path to unifying even current web and native app development, so that we don't have to write three different apps for the same client -- browser, iOS and Android -- or at least don't have to write them all from scratch.

###USING THE DEMOS

This course of study was developed by someone who has struggled hard to learn Angular 2 through the online Angular documentation. While good so far as it goes, and even excellent in some instances, it suffers from some critical weakness in my opinion.

1. It begins with a Quickstart that is inherently focused on boilerplate setup which (for reasons that are presently unavoidable) is unusually burdensome and complicated. This is not only discouraging to the newcomer, who has created half-a-dozen files to achieve the barest "hello world" experience, but, more importantly, it fails to stress from the get-go that this boilerplate is of almost negligible significance compared to the Angular 2 concept base, which deserves the beginner’s most immediate attention.

2. The Tour of Heroes example does too much, even though it is built sequentially. The best method for climbing the “wall of ice” that Angular 2 presents to newcomers must be to build concepts step-by-step, but __without the necessity of making some larger project hang together__.

3. The individual instructive sections in the Angular docs __Basics__ and __Developer's Guide__ are properly focused on specific topics, and are great once one knows one's way around. But this assumes some general “30,000 ft” *gestalt* that separates the forest from the trees.

My purpose here has been to provide the __graduated, yet holistic picture__ that I wish I had. Our goal is to sense how Angular 2 hangs together and provides something far more powerful and interesting than the sum of its manifold parts.

My personal advice is to get everything you can out of the demos themselves --  __pouring over the code before reading any of the attached explanations__ revealed by the __info__ button in the right-side panel. Only the files in the __app/__ folders will matter until much later the in sequence of demos. The boilerplate setup files rarely change from demo to demo, and when they do, this will be clearly stressed in the explanatory text.

I have provided very little commenting within the files. I find that once a comment tells me what I'm supposed to think about some line of code, I don't bother to think it through myself. That's fine for knowledge-sharing when developing in teams (or just refeshing your own memory), but it can be a barrier to true learning.

###TYPESCRIPT

 Angular 2 was designed to be written in TypeScript. So what is TypeScript? And does it really mean having to learn a new language or dialect in order to use Angular 2?

TypeScript is fantastic. It allows you to write JavaScript as though all of the expected and desired extensions to that language were already in effect, and then __transpiles (compiles)__ your code into EcmaScript 5 so that all current browsers understand it. Angular 2 uses, right now, so much of what is sure to be the future of the official JavaScript (EcmaScript) language, that TypeScript is essential. Just being able to write classes as real classes, and not as mere JavaScript constructors is enough, but there is much, much more.

TypeScript combines this expanded JavaScript langauge with __OPTIONAL__ type declarations. It is a final mark of maturity for JavaScript development that the loose-typing character of the language is no longer considered an advantage, at least in serious application development. It should __matter__ whether a variable (or an argument or return value) is a __string__ as opposed to a __number__ or a __boolean__, and we should be able to declare it so, both for greater comprehension when reading code and to allow the compiler to catch type conflicts (such as where a __string__ is assigned to a variable declared as an __array__).

The key word here is __OPTIONAL__. Don't want to use type definitions when you are just getting started with Angular 2? No problem! In fact, I agree wholeheartedly. Thus these demos only begin to introduce type declarations after a while, and only selectively, to introduce their value as it becomes obvious. Our primary goal is to learn some pretty challenging general Angular 2 concepts, and type definitions will add only clutter our code with unnecessary distractions at the start.

###LINKS TO PLUNKER DEMOS (and GITHUB REPOS)

[**Plunker Demo #1**](http://plnkr.co/edit/4A4juKPbXMrWzObNNal1?p=info)
-- SIMPLEST POSSIBLE COMPONENT (NON-DYNAMIC)
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo1)

[**Plunker Demo #2**](http://plnkr.co/edit/NGKu8NABbTi5ahCA1Rfu?p=info)
-- SIMPLEST POSSIBLE COMPONENT (DYNAMIC)
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo2)

[**Plunker Demo #3**](http://plnkr.co/edit/rya1huZwrmBDCjmXt9YB?p=info)
-- PROPERTY BINDING (COMPONENT TO DOM)
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo3)

[**Demo #4**](http://plnkr.co/edit/T0irbgvOaPJ8yZthEKsi?p=info)
-- EVENT BINDING (DOM TO COMPONENT)
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo4)

[**Plunker Demo #5**](http://plnkr.co/edit/DvLyixMC6JialnAO1wwE?p=info)
-- CONDITIONAL DISPLAY WITH *ngIf DIRECTIVE
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo5)

[**Plunker Demo #6**](http://plnkr.co/edit/ab2z8SWgN3L3gOhDyTKm?p=info)
-- DISPLAYING LISTS WITH *ngFor "REPEATER"
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo6)

[**Plunker Demo #7**](http://plnkr.co/edit/ba19hRRCJnt4tuMtlqeb?p=info)
-- SELECTING AN ITEM FROM *ngFor LIST WITH EVENT BINDING
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo7)

[**Plunker Demo #8**](http://plnkr.co/edit/hDdvmwAlbndB4tLDBbJK?p=info)
-- PARENT-CHILD COMPONENT HIERARCHY (SIMPLEST CASE)
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo8)

[**Plunker Demo #9**](http://plnkr.co/edit/hWmGqwVcDzppLItjfRxc?p=info)
-- PARENT-CHILD PROPERTY BINDING THRU @Input
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo9)

[**Plunker Demo #10**](http://plnkr.co/edit/KAdnfBVIxf8UPEpR4Psy?p=info)
-- CHILD-PARENT EVENT BINDINg THRU @Output (EventEmitter)
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo10)

[**Plunker Demo #11**](http://plnkr.co/edit/Dvw9v1R1XR5gxzIuPD5x?p=info)
-- PARENT CALLS CHILD METHODS THRU LOCAL TEMPLATE VARIABLE (#)
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo11)

[**Plunker Demo #12**](http://plnkr.co/edit/lLJW4EodgMAdSTFPrdmf?p=info)
-- *ngFor LIST DISPLAY OF CUSTOM CHILD COMPONENTS
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo12)

[**Plunker Demo #13**](http://plnkr.co/edit/V9n4MUFNH3f72ZWtrEgR?p=info)
-- INTERACTIVE SELECTION FROM CHILD COMPONENTS IN *ngFor LIST (EVENT PAYLOADS)
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo13)

[**Plunker Demo #14**](http://plnkr.co/edit/xmTaGvJwYGnOOcY2Movv?p=info)
-- APPLICATION STORE, SERVICE CLASSES & DEPENDENCY INJECTION (DI)
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo14)

[**Plunker Demo #15**](http://plnkr.co/edit/B0BUeGa63htHQcbPTfFK?p=info)
--RxJS SUBJECTS, OBSERVABLES & DATA STREAMS ("PUSHING" DATA EVENTS)
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo15)

[**Plunker Demo #16**](http://plnkr.co/edit/fRbQM1L5K7h3rexEbbVF?p=info)
-- TwO-WAY DATA BINDING BETWEEN COMPONENT PROPERTIES AND UI CONTROLS
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo16)

[**Plunker Demo #17**](http://plnkr.co/edit/3T6ru9k0Q7btqtuU4gBk?p=info)
-- INTRO TO ANGULAR 2 FORMS
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo17)

[**Plunker Demo #18**](http://plnkr.co/edit/qNEyPH7u6TFCjHQt2A11?p=info)
-- INTERACTIVE ADD AND DELETE OF *ngFor LIST ITEMS
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo18)

[**Plunker Demo #19**](http://plnkr.co/edit/ZexLiBgDhhNeXmGKAqRe?p=info)
-- INTRODUCING "DATABASE" PERSISTENCE (DATA FETCH SERVICE)
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo19)

[**Plunker Demo #20**](http://plnkr.co/edit/vvfj7SJNs0QU5crP5LuE?p=info)
--INTRO TO ROUTING and NAVIGATION
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo20)

[**Plunker Demo #21**](http://plnkr.co/edit/sHRVdLRdzpWnKedTmhkc?p=info)
-- DATA STORE TO INTEGRATE ROUTED APPLICATION
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo21)

[**Plunker Demo #22**](http://plnkr.co/edit/duxMpePu830kL8PWaBky?p=info)
-- USING URL PATH ROUTE PARAMETERS TO FETCH SELECTED DATA OBJECT
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo22)

[**Plunker Demo #23**](http://plnkr.co/edit/ROGwUMyApPMSY6y84Rpc?p=info)
-- SUBSCRIBING TO A ROUTE.PARAMS OBSERVABLE (DATA STREAM)
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo23)

[**Plunker Demo #24**](http://plnkr.co/edit/SiSzC0qpn6ZIwnkmTXV9?p=info)
-- FETCHING DATA FROM "FAKE" HTTP RESTful "IN-MEMORY" BACKEND
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo24)

[**Plunker Demo #25** (Optional/Extra Credit)](http://plnkr.co/edit/H01XXpEztaaehMNBhOZw?p=info)
-- FETCHING DATA FROM FIREBASE HTTP NETWORK BACKEND (RESTful-ish)
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo25)

[**Plunker Demo #26** (Optional/Extra Credit)](http://plnkr.co/edit/Uk4H1sJLxl4WWCrWZoZh?p=info)
-- FETCHING DATA FROM FIREBASE NETWORK "REAL-TIME" DATA SUBSCRIPTION (NO HTTP, NO REST API)
-- [**Github Repo**](https://github.com/rpolevoi/ngMind-beginner.mind_Demo26)

COMMENTS, BUGS, SUGGESTIONS, Etc.?  email robert.polevoi@gmail.com

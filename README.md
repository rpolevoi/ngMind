# ngMind="beginner.mind"

A __progressive course__ of 26 __ANGULAR 2__ plunker demos to master core integrated concepts before writing a word of code.

Complete list of demo-links is at the bottom of this doc.

(You can jump to first demo here below, but *please* try reading this Intro doc first -- it's well worth 10 minutes):

[**Demo #1**](http://plnkr.co/edit/4A4juKPbXMrWzObNNal1?p=info target="_blank")
-- SIMPLEST POSSIBLE COMPONENT (NON-DYNAMIC)

###INTRO

The title of these demos honors Shenryu Suzuki's "Zen Mind, Beginner Mind," in which the author makes an important observation for those approaching Angular 2. He stresses a willingness to cast off past accomplishments and expertise, and embrace the innocence of a true novice to embrace creative energies. *“In the beginner’s mind"* he says famously, *"there are many possibilities, but in the expert’s there are few.”* This insight is traceable to ancient Chinese thought, where Confucius stressed daily renewal and Mencius exhorted unrelenting efforts to recover our "original nature" which he so beautifully compares with the fresh, life-giving air of early dawn.

Speaking practically, there's an arguably real advantage for the novice developer when learning Angular 2 because he or she doesn't have to throw away much calcified achievement. Angular 2 is revolutionary at many fundamental conceptual levels, and the experienced developer cannot help but assimilate it through the filters of his or her own expertise. This will almost certainly be limiting in both learning and developing with Angular 2. The worst case, perhaps, is proficiency in Angular 1 because it is entirely counterproductive to build an Angular 2 mindset atop the karma of deep Angular 1 expertise. Angular 2 is a whole new animal, best approached with the most open possible mind. But even a snail is smart enough to shed its shell when it becomes confining.

###WHY LEARN ANGULAR 2?

Angular 2 is heavy lifting for anyone approaching it, no matter how impressive their cerebral equipment. In fact, it sometimes feels like climbing up a wall of ice. Thus it's fair to ask why one should take the time and risk to study it with the intensity that it demands. If the answer here seems long, consider the importance of the question.

Angular 2 is, to my mind, a very big thing. Bigger than Angular 1, bigger than Rails. It's no mere framework, but a __platform__. By framework, I mean an integrated set of tools that enable one to do much more efficiently what one could ultimately do themselves in a straight programming language like JavaScript or Ruby. A __platform__ is a much more ambitious concept. In this respect Angular 2 must be compared to the Windows operating system or, more accurately, to Java, as creating a fundamental technological foundation for new kinds of development, with a potential lifespan measured in decades. Like both both Windows and Java, the association with an extremely important (if not dominant) high-tech enterprise is critical, not least for leadership and the potential for an industry standard. It's simply impossible that Google will betray the global development community by failing to support and press forward with the Angular project, long past version 2. And its motives for doing so are more powerful than mere *noblesse oblige* or good developer relations, as we will see.

Microsoft had a huge practical stake in the success of Windows development because sales of the operating system was its bread and butter. Sun had an important stake in Java because it believed that a continuing market for its high-priced servers depended on its prescient vision of a future __internet of applications__, instead of static web pages. This vision never ended up working out on the client (through so-called applets) but saw considerable success on the server-side. And Java was both a first-class programming language and a technology (the Java Virtual Machine) that bridged across operating systems. The comparison to Angular 2 is obvious. Its language may be, strictly speaking, JavaScript (although written in TypeScript), but there is so much intellectual and syntactic superstructure that the underlying language ends up buried under uniquely Angular code and thought patterns. And the technology is the browser. Of course, the browser need not be Chrome or any implementation of Google V8 JavaScript engine. But no one understands the browser and JavaScript interpretation the way that Google does, and only Google could possibly tap into such expertise to create a platform like Angular 2 -- because the bottom line is solving a most fundamental problem: that of transparently connecting JavaScript code to the browser DOM in a way that really works. When an Angular developer binds a JavaScript property to a DOM property, he or she can feel confident that the latter will always reflect the value of the former, and that this convenience (which inherently involves a great deal of under-the-hood complexity) will come at no or negligible cost to performance. This heralds the end of the entire __jQuery__ era of JavaScript-DOM integration.

But Angular 2 is also Google's attempt to prod, shape and anticipate the future scale and possibilities of __web development as true application development__, just as Sun's vision was with Java. This goal accounts for almost all that is new, difficult, or even revolutionary in Angular 2. And, just as with Windows, there is a very serious business strategy here impacting Google as a whole, as is becoming increasing clear. With Angular 2, Google is taking aim at what, for it (and possibly for all of us) was the great disaster of mobile development. Apple played a disproportionate strategic role in mobile because it was first to market with the truly successful products and Steve Jobs was determined not to create another version of the browser-accessed internet (i.e., the World Wide Web) where everything was free or stealable. He decided that the mobile experience would live within locally-installed applications (on the older model of the desktop), downloaded from a “store” over which his company had exclusive control. He expected people to pay for their apps for the most part, and for Apple to share in this revenue just as it shared in revenue from music downloads.

There was, certainly at first, a valid technological argument for this as well, because short battery life, limited memory and processing power, and weak and expensive wireless service all converged to argue for downloading and installing an app only once for any given version, and loading it from local memory, only tapping data access from the internet as needed. Against this background, Google could do nothing more than launch the a competing OS, Android, to prevent Apple from dominating mobile completely, but this strategy never made sense for the company's crown jewel and moneymaker -- web search -- because mobile apps, living outside the browser were neither searchable nor could they search. Add to this the issue of forcing mobile development down a completely different path than web development, using languages other than JavaScript -- and with iOS and Android requiring divergent languages. In short, mobile app development is way too difficult, too expensive, and unsearchable. The ultimate absurdity is the general practice of companies duplicating their web sites as iOS and Android apps on the assumption that mobile users are more used to using installed apps than using their mobile browsers. With the incredible flood of apps appearing every day, the need for universal Google search to provide them with visibility is glaringly obvious, and the makeshift answers offered now as stopgaps aren't satisfactory.

The only real answer is to "degrade and ultimately destroy" the native mobile app as we know it, and replace it with what Google calls the __"progressive web app__." This model for development, which works right now in primitive examples, involves matching the current user experience in native mobile apps, but in a __web app living in the browser__. __Instant loading__ of at least the interface from browser storage. __Offline capabilities__, especially during wireless service interruptions. The __appearance of a dedicated app__, with browser features hidden unless demanded. All this and more. And most important are the **killer features mobile apps cannot pretend to offer**: __deep-linking of urls assigned to application state views__. A user can copy an url, even from deep within the app, and send it (for example) in an email as a link, where it can move to social media or web sites. And Google can find such links and make them searchable. The mobile experience thus breaks through the prison of its walled garden to engage the world. That this is critical for Google is too obvious for comment, because Google search has been shut out of mobile, where everyone agrees the great majority of user growth will continue to flourish. But it is also good for all of us, and particularly for developers who are already aware of how brutal it is to obtain any visibility for new mobile apps in such a crowded universe without the help of Google Search.

Should you doubt if this is really the most salient motive for Google with Angular 2 -- as the __ideal platform for displacing native mobile apps with searchable web apps__ -- check out the primary position given to progressive web apps on the Angular website Features page. In fact, Google goes much further, stressing that Angular is a clear path to unifying even web and native app development, so that we don't have to write three different apps for the same client -- browser, iOS and Android -- or at least don't have to write them all from scratch. Another key to Google's motivations in Angular 2 has been the obsessive pursuit of perfection on the subject of __routing__, holding up release of the entire project for months. Routing is the means for providing url links for application states and for __splitting up code downloads__ on an "as needed" basis that's especially useful over mobile connections.

This, believe it or not, is the shortest responsible answer to the question of why to bother learning Angular 2. Other answers might include the sheer exposure to the workings of the Google brain trust, which must always represent a kind of gold standard. Anyone who doesn't want to learn everything they can from Google own developers is missing something somewhere.

###USING THE DEMOS

This course of study was developed by someone who has made the most serious efforts to learn Angular 2 through the online Angular documentation. While good so far as it goes, and even excellent in some instances, it suffers from some critical weakness in my opinion.

1. It begins with a quickstart that is inherently focused on boilerplate setup which, for reasons mentioned below, is unusually burdensome and complicated. This is not only discouraging to the newcomer, but it fails to stress from the start that this boilerplate is of almost negligible significance compare of the Angular 2 concept base, which deserves the beginner’s most immediate attention.

2. The Tour of Heros example does too much, even though it is built sequentially. The best method for climbing the “wall of ice” that Angular 2 presents to newcomers must be to build concepts step-by-step, but __without the necessity of making a larger project hang together__.

3. The individual instructive sections are properly focused on individual topics, and are great once one knows the way around. But that assumes some general “30,000 ft” *gestalt* that separates the forest from the trees.

My purpose here has been to provide the graduated, yet holistic picture that I wish I had while spending weeks and months on Angular 2. The idea is to move progressively through the basic concepts, because an integrated sense of these concepts, even in a shallow way, is more important for the beginner that a strong grasp of any one of them. The point is to sense -- intuitively as much as consciously -- how Angular hangs together and provides something far more powerful and interesting than the sum of its parts.

My personal advice is to get everything you can out of the demos themselves --  __pouring over the code before reading any of the attached __explanation__ revealed by the __info__ button in the rightmost side panel. Only the files in the __app/__ folders will matter until much later the in sequence of demos. The boilerplate setup files do rarely change from demo to demo, and when they do, this will be clearly stressed in the explanatory text.

I have provided very little commenting within the files. The purpose is to give you the opportunity to figure out as much as you can from the bare code before turning to the explanations. I find that once a comment tells me what I've supposed to think about some line or block of code, or what it’s supposed to do, I don't bother to think it through myself. Perhaps you agree.

###TYPESCRIPT

Despite what the Angular 2 docs say, using straight JavaScript (much less Dart) to develop in Angular is ridiculous. Angular 2 was designed to be written in TypeScript, and nothing else makes sense. So what is TypeScript? And does it really mean having to learn a new language or dialect in order to use Angular 2?

TypeScript is fantastic. It allows you to write JavaScript as though all of the expected and desired extensions to that language were already in effect, and then __transpiles (compiles)__ your code into EcmaScript 5 so that all current browsers understand it. Angular 2 uses, right now, so much of what is sure to be the future of the official JavaScript (EcmaScript) language, that TypeScript is essential. Just being able to write classes as real classes, and not as mere JavaScript constructors is enough, but there is much, much more.

There are other transpilers out there that are well-respected. The advantage for TypeScript is that it combines transpiling with __OPTIONAL__ type declarations. It is a final mark of maturity for JavaScript development that the loose-typing character of the language is no longer considered an advantage, at least in serious application development. It should __matter__ whether a variable (or an argument or return value) is a __string__ as opposed to a __number__ or a __boolean__, and we should be able to declare it so, both for greater comprehension when reading code and to allow the compiler to catch type conflicts (such as where a __string__ is assigned to a variable declared as an __array__).

The key word here is __OPTIONAL__. Don't want to use type definitions when you are just getting started with Angular 2? No problem! In fact, I agree wholeheartedly. Thus these demos only begin to introduce type declarations after a while, and only selectively, to introduce their value as it becomes obvious. Our primary goal is to learn some pretty challenging general Angular 2 concepts, and type definitions will add only clutter our code with unnecessary distractions at the start.

###LINKS TO DEMOS

[**Demo #1**](http://plnkr.co/edit/4A4juKPbXMrWzObNNal1?p=info target="_blank")
-- SIMPLEST POSSIBLE COMPONENT (NON-DYNAMIC)

[**Demo #2**](http://plnkr.co/edit/NGKu8NABbTi5ahCA1Rfu?p=info target="_blank")
-- SIMPLEST POSSIBLE COMPONENT (DYNAMIC)

[**Demo #3**](http://plnkr.co/edit/rya1huZwrmBDCjmXt9YB?p=info target="_blank")
-- PROPERTY BINDING (COMPONENT TO DOM)

[**Demo #4**](http://plnkr.co/edit/T0irbgvOaPJ8yZthEKsi?p=info target="_blank")
-- EVENT BINDING (DOM TO COMPONENT)

[**Demo #5**](http://plnkr.co/edit/DvLyixMC6JialnAO1wwE?p=info target="_blank")
-- CONDITIONAL DISPLAY WITH *ngIf DIRECTIVE

[**Demo #6**](http://plnkr.co/edit/ab2z8SWgN3L3gOhDyTKm?p=info target="_blank")
-- DISPLAYING LISTS WITH *ngFor "REPEATER"

[**Demo #7**](http://plnkr.co/edit/ba19hRRCJnt4tuMtlqeb?p=info target="_blank")
-- SELECTING AN ITEM FROM *ngFor LIST WITH EVENT BINDING

[**Demo #8**](http://plnkr.co/edit/hDdvmwAlbndB4tLDBbJK?p=info target="_blank")
-- PARENT-CHILD COMPONENT HIERARCHY (SIMPLEST CASE)

[**Demo #9**](http://plnkr.co/edit/hWmGqwVcDzppLItjfRxc?p=info target="_blank")
-- PARENT-CHILD PROPERTY BINDING THRU @Input

[**Demo #10**](http://plnkr.co/edit/KAdnfBVIxf8UPEpR4Psy?p=info target="_blank")
-- CHILD-PARENT EVENT BINDINg THRU @Output (EventEmitter)

[**Demo #11**](http://plnkr.co/edit/Dvw9v1R1XR5gxzIuPD5x?p=info target="_blank")
-- PARENT CALLS CHILD METHODS THRU LOCAL TEMPLATE VARIABLE (#)

[**Demo #12**](http://plnkr.co/edit/lLJW4EodgMAdSTFPrdmf?p=info target="_blank")
-- *ngFor LIST DISPLAY OF CUSTOM CHILD COMPONENTS

[**Demo #13**](http://plnkr.co/edit/V9n4MUFNH3f72ZWtrEgR?p=info target="_blank")
-- INTERACTIVE SELECTION FROM CHILD COMPONENTS IN *ngFor LIST (EVENT PAYLOADS)

[**Demo #14**](http://plnkr.co/edit/xmTaGvJwYGnOOcY2Movv?p=info target="_blank")
-- APPLICATION STORE, SERVICE CLASSES & DEPENDENCY INJECTION (DI)

[**Demo #15**](http://plnkr.co/edit/B0BUeGa63htHQcbPTfFK?p=info target="_blank")
--RxJS SUBJECTS, OBSERVABLES & DATA STREAMS ("PUSHING" DATA EVENTS)

[**Demo #16**](http://plnkr.co/edit/fRbQM1L5K7h3rexEbbVF?p=info target="_blank")
-- TwO-WAY DATA BINDING BETWEEN COMPONENT PROPERTIES AND UI CONTROLS

[**Demo #17**](http://plnkr.co/edit/3T6ru9k0Q7btqtuU4gBk?p=info target="_blank")
-- INTRO TO ANGULAR 2 FORMS

[**Demo #18**](http://plnkr.co/edit/qNEyPH7u6TFCjHQt2A11?p=info target="_blank")
-- INTERACTIVE ADD AND DELETE OF *ngFor LIST ITEMS

[**Demo #19**](http://plnkr.co/edit/ZexLiBgDhhNeXmGKAqRe?p=info target="_blank")
-- INTRODUCING "DATABASE" PERSISTENCE (DATA FETCH SERVICE)

[**Demo #20**](http://plnkr.co/edit/vvfj7SJNs0QU5crP5LuE?p=info target="_blank")
--INTRO TO ROUTING and NAVIGATION

[**Demo #21**](http://plnkr.co/edit/sHRVdLRdzpWnKedTmhkc?p=info target="_blank")
-- DATA STORE TO INTEGRATE ROUTED APPLICATION

[**Demo #22**](http://plnkr.co/edit/duxMpePu830kL8PWaBky?p=info target="_blank")
-- USING URL PATH ROUTE PARAMETERS TO FETCH SELECTED DATA OBJECT

[**Demo #23**](http://plnkr.co/edit/ROGwUMyApPMSY6y84Rpc?p=info target="_blank")
-- SUBSCRIBING TO A ROUTE.PARAMS OBSERVABLE (DATA STREAM)

[**Demo #24**](http://plnkr.co/edit/SiSzC0qpn6ZIwnkmTXV9?p=info target="_blank")
-- FETCHING DATA FROM "FAKE" HTTP RESTful "IN-MEMORY" BACKEND

[**Demo #25** (Optional/Extra Credit)](http://plnkr.co/edit/H01XXpEztaaehMNBhOZw?p=info target="_blank")
-- FETCHING DATA FROM FIREBASE HTTP NETWORK BACKEND (RESTful-ish)

[**Demo #26** (Optional/Extra Credit)](http://plnkr.co/edit/Uk4H1sJLxl4WWCrWZoZh?p=info target="_blank")
-- FETCHING DATA FROM FIREBASE NETWORK "REAL-TIME" DATA SUBSCRIPTION (NO HTTP, NO REST API)

COMMENTS, BUGS, SUGGESTIONS, Etc.?  email robert.polevoi@gmail.com

# awesome-js-memory
Ресурсы про память и утечки в JavaScript

Теория
------
[Memory Management Reference](https://www.memorymanagement.org/) - общая теория об устройстве памяти  
[MDN Memory Management](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Memory_Management) - короткая статья про память в js  
[Сборщик мусора в V8, иллюстрированное руководство](https://medium.com/devschacht/%D1%81%D0%B1%D0%BE%D1%80%D1%89%D0%B8%D0%BA-%D0%BC%D1%83%D1%81%D0%BE%D1%80%D0%B0-%D0%B2-v8-%D0%B8%D0%BB%D0%BB%D1%8E%D1%81%D1%82%D1%80%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%BD%D0%BE%D0%B5-%D1%80%D1%83%D0%BA%D0%BE%D0%B2%D0%BE%D0%B4%D1%81%D1%82%D0%B2%D0%BE-d3e496a4d378) - перевод статьи Ирины Шестак  
[Understanding Javascript Function Executions — Call Stack, Event Loop , Tasks & more](https://medium.com/@gaurav.pandvia/understanding-javascript-function-executions-tasks-event-loop-call-stack-more-part-1-5683dea1f5ec), Gaurav Pandvia - отличная иллюстрация работы стека, кучи и цикла событий в js  
[How variables are allocated memory in Javascript?](https://stackoverflow.com/questions/2800463/how-variables-are-allocated-memory-in-javascript) - отличный ответ со stackoverflow  
[Confused about Stack and Heap?](https://medium.com/fhinkel/confused-about-stack-and-heap-2cf3e6adb771), Franziska Hinkelmann - чем стек отличается от кучи на пальцах  
[A New Way to Debug Memory Issues with Web Apps](https://medium.com/@tomlagier/a-new-way-to-debug-memory-issues-with-web-apps-4e29df964af2), Tom Lagier - красивая визуализация кучи js  
[Choosing a Visualization Method for Memory Profiles](https://hackernoon.com/a-tale-of-javascript-performance-6011615523e8), Tom Lagier - различные способы визуализировать память в js  
  

Про утечки памяти
-----------------
[How To Write Fast, Memory-Efficient JavaScript](https://www.smashingmagazine.com/2012/11/writing-fast-memory-efficient-javascript/), Addy Osmani  
[A toddlers guide to memory leaks in Javascript](https://dev.to/kepta/a-toddlers-guide-to-memory-leaks-in-javascript-25lf), Kushan Joshi - про утечки памяти для маленьких  
[Beyond Memory Leaks in JavaScript](https://medium.com/outsystems-experts/beyond-memory-leaks-in-javascript-d27fd48ae67e), Daniel Reis - вводная статья про память и утечки с гифками и танцами  
[Memory leaks and memory management in JavaScript](https://antongorbikov.wordpress.com/2015/08/27/about-memory-leaks-again/), Anton Gorbikov  
[4 Types of Memory Leaks in JavaScript and How to Get Rid Of Them](https://auth0.com/blog/four-types-of-leaks-in-your-javascript-code-and-how-to-get-rid-of-them/), Sebastián Peyrott - про типовые причины утечек памяти, [[перевод](https://habr.com/post/309318/)]  
[Как находить и устранять утечки памяти на примере Яндекс.Почты](https://habr.com/company/yandex/blog/195198/)  
[Be careful with console logs](https://medium.com/@cherniavskii/javascript-console-log-memory-leak-de3433efb278), Andrew Cherniavski - про утечки памяти из-за js-консоли  
[How JavaScript works: memory management + how to handle 4 common memory leaks](https://blog.sessionstack.com/how-javascript-works-memory-management-how-to-handle-4-common-memory-leaks-3f28b94cfbec), Alexander Zlatkov - про типичные причины утечек, [[перевод](https://habr.com/company/ruvds/blog/338150/)]  
[Hunting JS memory leaks in React Native apps](https://blog.swmansion.com/hunting-js-memory-leaks-in-react-native-apps-bd73807d0fde), Krzysztof Magiera  
[Hunting Memory Leaks in Backbone](https://content.pivotal.io/blog/hunting-memory-leaks-in-backbone), Charles Hansen  
[Simple Guide to Finding a JavaScript Memory Leak in Node.js](https://www.alexkras.com/simple-guide-to-finding-a-javascript-memory-leak-in-node-js/), Alex Kras  
[Fixing Memory Leaks in AngularJS and other JavaScript Applications](https://www.dwmkerr.com/fixing-memory-leaks-in-angularjs-applications/), Dave Kerr  
[Understanding Garbage Collection and hunting Memory Leaks in Node.js](https://www.dynatrace.com/news/blog/understanding-garbage-collection-and-hunting-memory-leaks-in-node-js/), Daniel Khan - про gc и утечки памяти в node.js  

Автоматизация
-------------
[SeaLant](https://github.com/saby/SeaLant) - фреймворк на Python для выявление утечек памяти через тесты на Selenium  
[Drool](https://github.com/samccone/drool) - выявляет утечки DOM и подписок  
[BLeak](https://github.com/plasma-umass/BLeak) - выявление утечек памяти во фронтенде [описние](https://jvilk.com/assets/pdf/bleak.pdf), официальный [сайт](http://plasma-umass.org/BLeak/)  
[Browser’s Memory Profiling Automation](http://www.theseus.fi/bitstream/handle/10024/133482/Browsers%20Automated%20Memory%20Profiling.pdf;jsessionid=BC27E5B30358CA5ED1C302468642EA94?sequence=1), Lucy Liu - достаточно подробное описание процесса автоматизации  
[Watson](https://github.com/airhorns/watson) - исследует производительность js в целом и утечки памяти в частности  
[memdiff](https://github.com/azer/memdiff) - юнит-тесты для обнаружения утечек памяти  
[Automatic leak detection for V8 heap snapshots](https://github.com/joyeecheung/v8-mat) - помогает по снапшоту v8 понять, кто виноват в утечке  
[Leakage](https://github.com/andywer/leakage) - ещё один инструмент для выявления утечек памяти в node.js  

Браузеры и движки
-----------------
[Memory in Chromium](https://chromium.googlesource.com/chromium/src/+/master/docs/memory/README.md) - всё про работу с памятью в проекте Chromium  
[v8-perf](https://github.com/thlorenz/v8-perf) - профилирование производительности в движке v8  
[v8 documentation](https://v8.dev/docs)  
[Isolating memory leaks with Chrome’s Allocation Timeline](https://blog.logrocket.com/isolating-memory-leaks-with-chromes-allocation-timeline-244fa9c48e8e), Renzo Lucioni  
[Taming The Unicorn: Easing JavaScript Memory Profiling In Chrome DevTools](https://addyosmani.com/blog/taming-the-unicorn-easing-javascript-memory-profiling-in-devtools/), Addy Osmani  
[Fix Memory Problems in Chrome DevTools](https://developers.google.com/web/tools/chrome-devtools/memory-problems/)  
[Memory in Edge](https://docs.microsoft.com/en-us/microsoft-edge/devtools-guide/memory) - про анализ памяти в браузере от microsoft  
[Firefox](https://wiki.mozilla.org/DevTools/Memory/Roadmap#Performance_Tools) - вики статья про инструменты анализа памяти в браузере Fx

Презентации
-----------
[Finding and debugging memory leaks in JavaScript with Chrome DevTools](http://slides.com/gruizdevilla/memory#/), Gonzalo Ruiz de Villa  
[A Trip Down Memory Lane with Gmail and Chrome DevTools](https://www.youtube.com/watch?v=x9Jlu_h_Lyw) (2013) [42min] - доклад с Google I/O и связанная презентация [BloatBusters: Eliminating memory leaks in Gmail](https://docs.google.com/presentation/d/1wUVmf78gG-ra5aOxvTfYdiLkdGaR9OhXRnOlIcEmu2s/pub?start=false&loop=false&delayms=3000&slide=id.g1d65bdf6_0_0), Loreena Lee и Robert Hundt  
[Memory Management Masterclass with Addy Osmani](https://www.youtube.com/watch?v=LaxbdIyBkL0) (2014) [55min] - доступны [слайды](https://speakerdeck.com/addyosmani/javascript-memory-management-masterclass) и [примеры кода](https://github.com/addyosmani/memory-mysteries)  
[The Breakpoint, Ep. 8: Memory Profiling with Chrome DevTools](https://www.youtube.com/watch?v=L3ugr9BJqIs) (2013) [26min]  
[Profiling in the wild by Sam Saccone](https://www.youtube.com/watch?v=OLWEyH7_4e0) (2015) [8min]  

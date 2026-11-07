---
title: "How One CPU Runs Many Programs: Context Switching"
excerpt: "My presentation for the English course"
permalink: /context-switching/
---

## About this talk

A computer runs a browser, music and a chat app at the same time, but one CPU core can run only one program at a time. How is this possible? The answer is the **context switch**: the operating system saves the state of one process and loads the state of another, many times every second.

In this talk I explain three things:

1. **What is it?** Processes, the PCB and the idea of a context switch.
2. **How does it work?** The steps inside the operating system, with examples from Windows and Linux.
3. **What does it cost?** The time of one switch, the hidden cost of a cold cache, and how to see context switches on your own computer.

**Date:** 12 November 2026 · **Length:** about 10 minutes

## Slides

<div class="deck-cards">
  <a class="deck-card" href="{{ '/slides/context-switching/' | relative_url }}">
    <div class="deck-card__media">
      <img src="{{ '/assets/slides/cs-animated.png' | relative_url }}" alt="First slide of the animated presentation" loading="lazy">
      <span class="deck-card__play"><i class="fas fa-play"></i></span>
      <span class="deck-card__badge"><i class="fas fa-wand-magic-sparkles"></i> Animated</span>
    </div>
    <div class="deck-card__body">
      <strong>Animated slides</strong>
      <span>Opens in the browser · full screen button inside</span>
    </div>
  </a>
  <a class="deck-card" href="{{ '/assets/slides/context-switching.pdf' | relative_url }}" target="_blank" rel="noopener">
    <div class="deck-card__media">
      <img src="{{ '/assets/slides/cs-pdf.png' | relative_url }}" alt="A slide from the PDF version" loading="lazy">
      <span class="deck-card__play"><i class="fas fa-file-pdf"></i></span>
      <span class="deck-card__badge"><i class="fas fa-file-pdf"></i> PDF</span>
    </div>
    <div class="deck-card__body">
      <strong>PDF slides</strong>
      <span>15 slides · opens in a new tab</span>
    </div>
  </a>
</div>

## Sources

<ol class="src-list">
  <li><span class="src-tag">Paper</span><a href="https://web.stanford.edu/~ouster/cgi-bin/papers/osfaster.pdf" target="_blank" rel="noopener">Ousterhout, J. (1990). Why Aren't Operating Systems Getting Faster As Fast as Hardware? USENIX Summer Conference.</a></li>
  <li><span class="src-tag">Paper</span><a href="https://www.cs.rochester.edu/~kshen/papers/expcs2007.pdf" target="_blank" rel="noopener">Li, C., Ding, C. &amp; Shen, K. (2007). Quantifying the Cost of Context Switch. ACM Workshop on Experimental Computer Science (ExpCS).</a></li>
  <li><span class="src-tag">Book</span><a href="https://pages.cs.wisc.edu/~remzi/OSTEP/cpu-mechanisms.pdf" target="_blank" rel="noopener">Arpaci-Dusseau, R. &amp; Arpaci-Dusseau, A. Operating Systems: Three Easy Pieces, Chapter 6: Limited Direct Execution.</a></li>
  <li><span class="src-tag">Tech doc</span><a href="https://learn.microsoft.com/en-us/windows/win32/procthread/context-switches" target="_blank" rel="noopener">Microsoft Learn. Context Switches.</a></li>
  <li><span class="src-tag">Tech doc</span><a href="https://docs.kernel.org/scheduler/sched-design-CFS.html" target="_blank" rel="noopener">Linux Kernel Documentation. CFS Scheduler</a> &amp; <a href="https://docs.kernel.org/scheduler/sched-eevdf.html" target="_blank" rel="noopener">EEVDF Scheduler.</a></li>
  <li><span class="src-tag">Blog</span><a href="https://eli.thegreenplace.net/2018/measuring-context-switching-and-memory-overheads-for-linux-threads/" target="_blank" rel="noopener">Bendersky, E. (2018). Measuring context switching and memory overheads for Linux threads.</a></li>
  <li><span class="src-tag">Blog</span><a href="https://blog.tsunanet.net/2010/11/how-long-does-it-take-to-make-context.html" target="_blank" rel="noopener">Sigoure, B. "tsuna" (2010). How long does it take to make a context switch?</a></li>
  <li><span class="src-tag">Code</span><a href="https://github.com/gz/contextswitch" target="_blank" rel="noopener">gz/contextswitch: a small program that measures context switch time (GitHub).</a></li>
  <li><span class="src-tag">Tutorial</span><a href="https://www.geeksforgeeks.org/operating-systems/context-switch-in-operating-system/" target="_blank" rel="noopener">GeeksforGeeks. Context Switch in Operating System.</a></li>
</ol>

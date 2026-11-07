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
      <img src="{{ '/assets/slides/cs-animated.webp' | relative_url }}" width="960" height="540" alt="First slide of the animated presentation" loading="lazy">
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
      <img src="{{ '/assets/slides/cs-pdf.webp' | relative_url }}" width="960" height="540" alt="A slide from the PDF version" loading="lazy">
      <span class="deck-card__play"><i class="fas fa-file-pdf"></i></span>
      <span class="deck-card__badge"><i class="fas fa-file-pdf"></i> PDF</span>
    </div>
    <div class="deck-card__body">
      <strong>PDF slides</strong>
      <span>15 slides · 0.45 MB · opens in a new tab</span>
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
  <li><span class="src-tag">Tech doc</span><a href="https://man7.org/linux/man-pages/man8/vmstat.8.html" target="_blank" rel="noopener">Linux man-pages. vmstat(8)</a> &amp; <a href="https://man7.org/linux/man-pages/man5/proc_pid_status.5.html" target="_blank" rel="noopener">proc_pid_status(5).</a></li>
  <li><span class="src-tag">Tech doc</span><a href="https://learn.microsoft.com/en-us/windows/win32/cimwin32prov/win32-perfformatteddata" target="_blank" rel="noopener">Microsoft Learn. Win32_PerfFormattedData classes.</a></li>
  <li><span class="src-tag">Blog</span><a href="https://eli.thegreenplace.net/2018/measuring-context-switching-and-memory-overheads-for-linux-threads/" target="_blank" rel="noopener">Bendersky, E. (2018). Measuring context switching and memory overheads for Linux threads.</a></li>
</ol>

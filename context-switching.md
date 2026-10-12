---
title: "How One CPU Runs Many Programs: Context Switching"
excerpt: "My presentation for the English course"
permalink: /context-switching/
---

## About this talk

Coming soon.

## See it in action

<div class="cs-demo" data-run="a" data-pkt="">
  <div class="cs-stage">
    <div class="cs-node cs-a">
      <div class="cs-name"><span class="cs-dot"></span>Process A</div>
      <div class="cs-work"><i></i></div>
      <div class="cs-pcb"><b>PCB A</b>PC · SP · Regs</div>
    </div>
    <div class="cs-cpu">
      <div class="cs-chip"><i class="fas fa-microchip"></i><b>CPU</b><span class="cs-now">A</span></div>
      <span class="cs-irq"><i class="fas fa-bolt"></i></span>
    </div>
    <div class="cs-node cs-b">
      <div class="cs-name"><span class="cs-dot"></span>Process B</div>
      <div class="cs-work"><i></i></div>
      <div class="cs-pcb"><b>PCB B</b>PC · SP · Regs</div>
    </div>
    <span class="cs-packet">PC · SP · R1</span>
  </div>
  <p class="cs-caption">Process A is running on the CPU.</p>
  <div class="cs-steps"><span class="is-on"></span><span></span><span></span><span></span><span></span><span></span><span></span><span></span></div>
</div>

## Slides

<div class="info-card">
  <i class="fas fa-file-pdf"></i>
  <div>
    <strong>Slides will be uploaded here</strong>
    <span>one day before the presentation</span>
  </div>
</div>

## Sources

Coming soon.

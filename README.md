# p5-comfy-workshop

Workshop combining p5.js and ComfyUI, via RunComfy.com

---

## Overview

This is a workshop for combining p5.js and ComfyUI, deployed using cloud-based GPU servers at RunComfy.com. In this workshop, the canvas produced by simple generative code in p5.js is used to guide an img2img algorithm — effectively treating Stable Diffusion as a filter or renderer. The workshop is based on the [p5.comfyui-helper](https://github.com/gohai/p5.comfyui-helper) by [Gottfried Haider](https://github.com/gohai), the [comfyui-p5js-node](https://github.com/tracerstar/comfyui-p5js-node) by Benjamin Fox, and invaluable help from CMU BCSA student, [Lorie Chen](https://github.com/ylchen333/p5.comfyui-helper/tree/main?tab=readme-ov-file). For related work, see also my [p5-in-comfyui](https://github.com/golanlevin/p5-in-comfyui), [image analysis](https://github.com/golanlevin/60-212/tree/main/lectures/comfy/image_analysis), and [image synthesis](https://github.com/golanlevin/60-212/tree/main/lectures/comfy/image_synthesis) lessons. This workshop was initially prepared for a presentation to undergraduates in RISD's Computation, Technology, and Culture (CTC) program in October, 2025. 

---

## ComfyUI Setup 

These are instructions for configuring RunComfy.com to provide stable-diffusion image synthesis for the provided p5.js sketch example. 

---

## Workshop

### 0. Overview - Contents

1. Quick review of p5.js
 	* As used in generative art
 	* Some basic code
2. Introduction to Stable Diffusion
	* [More like this please](https://github.com/golanlevin/lectures/blob/master/lecture_cnns_and_gans/more-like-this-please.md)

---

### 1. p5.js Review

* How some artists are using p5.js for generative art ("more like this please"):
  * [Forecast](https://www.fxhash.xyz/project/forecast) by [Amy Goodchild](https://www.amygoodchild.com/about)
  * [*nth culture*](https://deca.art/collection/nth-culture-by-fingacode) by [Junior Ngoma](https://www.youtube.com/watch?v=2Lero3In5uc) (Fingacode)
  * [*Memories of Qilin*](https://www.artblocks.io/collection/memories-of-qilin-by-emily-xie) by [Emily Xie](https://emilyxie.art/about)
  * [*Fragments of an Infinite Field*](https://www.artblocks.io/collection/fragments-of-an-infinite-field-by-monica-rizzolli) by [Monica Rizzolli](https://monicarizzolli.io/)
  * [*Take Wing*](https://www.fxhash.xyz/project/take-wing) by [Melissa Wiederrecht](https://melissawiederrecht.com/about)
  * [*Turner Light*](https://www.fxhash.xyz/generative/slug/turner-light) by [Aluan Wang](https://aluanwang.com/)
* Introduction to some simple code structures for generativity
  * [The problem](https://editor.p5js.org/golan/sketches/q5z3EFQ31)
  * [Generate with a very low `frameRate()`](https://editor.p5js.org/golan/sketches/xkcseJy0d)
  * [Click to Generate using `redraw()`](https://editor.p5js.org/golan/sketches/njx4cWSRf)
  * [Click to Generate using `randomSeed()`](https://editor.p5js.org/golan/sketches/HmynAX3EA)
* Review of [slider UI elements](https://editor.p5js.org/golan/sketches/f0RthyKYM)
* Review of [randomness]()
* Review of string assembly


### 2. Introduction to Stable Diffusion

* [More Like This, Please](https://github.com/golanlevin/lectures/blob/master/lecture_cnns_and_gans/more-like-this-please.md) (With AI)
	* Contrasting older and newer approaches to generative art
	* Programming with examples, not instructions
* [Bare-bones Diffusion Models explanation](https://madebyoll.in/posts/dino_diffusion/) by Ollin Boer Bohan (2023)
	* *"Criteria for image generation: plausibility, proportionality, and originality"*
	* *"Image denoising solves image generation....Denoising-based generation works by iterative [pareidolia](img/pareidolia.png)."*
	* *"At each step of training, the network receives a new batch of randomly-selected noisified real images, tries its best to denoise them, checks its work against the real images, and gets a little bit better."*
* Interactive Diffusion explainer
	* [Dino-Diffusion explainer demo](https://madebyoll.in/posts/dino_diffusion/demo/) (Bohan)
	* [At openProcessing.org](https://openprocessing.org/sketch/2321795)
	* [At the editor.p5js.org](https://editor.p5js.org/golan/sketches/LeAHAOHgZ)





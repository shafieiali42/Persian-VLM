# Persian-VLM

This repository contains my implementation of **Persian CLIP** and **Persian Image Captioning** models, designed to improve vision-language tasks for the Persian language.

## Overview

Since the CLIP model does not perform well for Persian text, I implemented a **Persian CLIP model** by replacing the CLIP text encoder with **ParsBERT** and fine-tuning it using contrastive learning. Additionally, I used the learned image encoder to implement a **Persian image captioning model** using an RNN.

## Repository Structure

- **Persian CLIP (`Persian CLIP.ipynb`)**  
  - Implements CLIP for the Persian language.  
  - Uses **ParsBERT** as the text encoder.  
  - Fine-tuned using **contrastive learning**.  
  - Can be used for **zero-shot object detection, cross-modal retrieval (text-to-image and image-to-text search), and other vision-language applications**.

- **Persian Image Captioning (`Persian Image Captioning.ipynb`)**  
  - Uses the image encoder from Persian CLIP.  
  - Implements an **RNN-based image captioning model** for Persian.

## Applications

- **Zero-shot object detection**  
- **Image retrieval**  
- **Cross-modal retrieval (text-to-image and image-to-text search)**  
- **Persian image captioning**  

## Examples of Image Captioning

Here are some example outputs from the **Persian Image Captioning** model:



<table>
  <tr>
    <td align="center">
      <img src="assets/Ski.png" alt="Example 2" width="250" height="200">
      <p><strong>یک اسکی باز در حال اسکی کردن از تپه ای برفی است.</strong></p>
    </td>
     <td align="center">
      <img src="assets/Bazaar.png" alt="Example 2" width="300" height="200">
      <p><strong>مردم در یک بازار شلوغ در فضای باز</strong></p>
    </td>
    <td align="center">
      <img src="assets/Girls.png" alt="Example 2" width="300" height="200">
      <p><strong>سه دختر جوان د حال بازی با یکدیگر</strong></p>
    </td>
  <tr>
  <tr>
    <td align="center">
      <img src="assets/Dancing.png" alt="Example 2" width="250" height="200">
      <p><strong>گروهی از زنان در حال رقصیدن در یک سالن رقص هستند.</strong></p>
    </td>
    <td align="center">
      <img src="assets/Dogs.png" alt="Example 1" width="300" height="200">
      <p><strong>سه سگ در حال بازی در چمن</strong></p>
    </td>
    <td align="center">
      <img src="assets/Surfing.png" alt="Example 2" width="400" height="200">
      <p><strong>مردی با پیراهن آبی در حال پریدن از روی تخته موج سوار است.</strong></p>
    </td>
  </tr>
</table>

# Nahor: live demo

Nahor translates Word documents from English to Assamese. It keeps the layout, tables and pictures, protects the terms in your own glossary, and also makes a version that opens cleanly in Google Docs.

This repository contains only the **built web demo**. The full application, including the Python backend that controls the translation on Kaggle, is kept private.

Open the live demo from the link in the **Website** field of this repository (right side of this page).

## What the demo is

- The whole interface works: upload, glossary extraction, progress, results, My Workspace, settings, themes, phone layout.
- Nothing is sent anywhere. Your file is not read and no server is involved.
- Every translation returns the same prepared sample (a short passage on the Indian Constitution) so the full flow can be tried in under a minute.

## What the real application does

1. A Python (FastAPI) backend uploads your document to your own private Kaggle dataset.
2. A notebook on your free Kaggle GPU translates it with the IndicTrans2 model, keeping your approved glossary terms.
3. Results are downloaded as a Word file and a Google Docs friendly file, split automatically when large.

Stack: React 19 and Vite, FastAPI, Kaggle API, IndicTrans2, python-docx.

## Contact

Bikash Deka, krishnamonideka10@gmail.com

All rights reserved. See LICENSE.

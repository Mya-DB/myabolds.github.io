---
layout: page
title: Smart Mirror — Auditing Beauty Filters
description: A live deployment for studying how Instagram-style beauty filters reshape AI's read of race, age, gender, and emotion.
category: work
importance: 1
related_publications: false
---

As part of my graduate research at UC San Diego, I led a mixed-methods study that trained nine paired conditional GANs to replicate Instagram beauty-filter transformations, then directed a student team in building a **Smart Mirror** system — Java/HTML/CSS on the frontend, Python/Flask and SQL + Supabase underneath — to deploy those models in real time.

The system let participants see filtered versions of their own face live, while we collected user surveys and audited how the filter-induced changes shifted downstream AI predictions of race, age, gender, and emotion. A companion bias-auditing pipeline (computer vision, Python, pretrained models, statistical modeling) quantified how the filters altered facial features, and how much Western beauty standards shaped those changes.

This work is currently in submission as {% cite bolds2026mirrorlies %}.

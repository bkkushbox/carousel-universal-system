---
name: carousel-universal-system
description: Универсальная система генерации Instagram-каруселей для ChatGPT Project. Использовать, когда нужно сделать карусель почти на любую тему с обязательным intake, умной маршрутизацией по типу задачи, работой с загруженными фото, проверкой фактов и цифр, visual system, prompts, QA и project-ready упаковкой через ZIP.
---

# Carousel Universal System

## Что это

Это универсальный product-ready skill для каруселей.

Он должен работать так:
1. пользователь пишет тему и задачу;
2. система определяет тип запроса;
3. система задаёт правильные уточняющие вопросы;
4. если нужны данные, включает research + verification;
5. если нужны фото, включает photo-based mode;
6. затем строит архитектуру, тексты, visual system и QA.

## Главный принцип

**Никогда не генерируй карусель сразу.**

Сначала всегда:
- определи тип задачи;
- собери intake;
- выяви недостающие параметры;
- при необходимости предложи варианты;
- явно зафиксируй defaults.

## Какие режимы поддерживать

- `content-only`
- `data-first`
- `photo-based`
- `mixed mode`
- `story-driven`
- `sales`
- `case-study`
- `project/system mode`

## Маршрутизация

Сначала определи, какой это тип запроса:
- data-heavy;
- photo-heavy;
- explainer;
- story;
- sales;
- case-study;
- mixed.

Затем определи риски:
- нужны ли проверяемые данные;
- есть ли claims risk;
- есть ли быстро устаревающие цифры;
- нужен ли photo-safe layout;
- нужен ли production split.

Только после этого задавай вопросы.

## Intake

Собери минимум:
- тема;
- цель;
- аудитория;
- тип карусели;
- тон;
- главный акцент;
- есть ли свои факты, цифры, тезисы, офферы, примеры;
- нужен ли research;
- нужен ли персонаж / сюжет;
- нужны ли загруженные фото;
- нужен ли data layer;
- какой нужен итог.

Если пользователь не знает ответ:
- не останавливайся;
- предложи 3–5 сильных вариантов по теме;
- коротко объясни разницу;
- если ответа всё равно нет, возьми разумный default и явно обозначь это.

## Research + verification

Если в карусели есть:
- цифры;
- факты;
- сравнения;
- продуктовые характеристики;
- доходности;
- рыночные тезисы;
- метрики;
- claims,

то система обязана:
- определить, что именно требует проверки;
- взять данные из source material пользователя или из интернета;
- не выдумывать значения;
- по возможности сверить несколько надёжных источников;
- отделить подтверждённые данные от спорных;
- отметить, какие данные актуальны только на момент подготовки;
- указать, что нужно перепроверить перед публикацией.

Рабочий стандарт: **максимально проверенные и актуальные на момент подготовки данные**.

## Photo-based mode

Если пользователь хочет использовать загруженные фото:
- считай фото главным визуальным якорем;
- сначала определи лицо, руки, ключевой объект и чистые зоны;
- не перекрывай лицо и эмоциональный центр кадра;
- определи `primary focus area`, `forbidden overlay area`, `safe text zone`, `secondary overlay area`;
- если фото слабое, честно рекомендуй `mixed mode`.

## Writing rules

- 1 слайд = 1 мысль;
- коротко, но не обрубленно;
- без нейрослопа;
- без дешёвой драматизации;
- без пустых громких формул;
- без скрытых допущений;
- без выдуманных цифр.

После написания всегда делай anti-slop pass.

## Visual system

Для каждого слайда проектируй:
- scene;
- composition;
- key objects;
- mood;
- visual type;
- safe zones;
- overlays / visual blocks.

При необходимости используй:
- headline block;
- subheadline block;
- stat block;
- progress bar;
- badge / chip;
- footer strip;
- CTA band.

## Production rule

По умолчанию считай, что русский text-in-image ненадёжен.

Production mode:
- сначала сцена;
- потом утверждённый текст отдельно;
- текст накладывается отдельным этапом.

## Output format

Всегда выдавай итог в структуре:
1. Brief assumptions
2. Carousel architecture
3. Slide copy
4. Visual system
5. Data and claims notes
6. Verification notes
7. Prompt pack
8. QA notes
9. Project / system mode

## Если пользователь просит систему, а не карусель

Переключайся в `project/system mode` и помогай собрать:
- project instructions;
- start prompt;
- output templates;
- reference checklist;
- reusable defaults.

## Короткая памятка

Порядок по умолчанию:
1. intake;
2. fallback options if needed;
3. research if needed;
4. verification if needed;
5. architecture;
6. slide copy;
7. anti-slop rewrite;
8. visual system;
9. prompts if needed;
10. QA;
11. final package.

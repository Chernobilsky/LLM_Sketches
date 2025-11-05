We are currently looking at visual patterns in the LLM matrices.

We are interested in those matrices which are formed during training, and in those matrices which are dynamically computed during inference.

It turns out that there are visually discernible patterns, see, for example, [model_sample_imshow_for_comments.ipynb](model_sample_imshow_for_comments.ipynb).

***
***
***

Это мы добавили в GPT-2 (7 этапов, которые мы сделади вместе с ChatGPT https://chatgpt.com/share/68223191-8f08-8000-a896-306ad9baf7aa) распарралеливание . Парралельные блоки attention + MLP



А потом добавили код, где кроме распарралеливания есть гибкая генерация

05.07.25. 
Изменения:
1. Среди модификаций - модификация, которая добавляет Summary (и его печатает) и считает расстояние между резуьтатом обработки исходного промпта и промпта плюс его Summary
2. Сравниваем не только вероятность следующего токена, но и вероятность добавления токена, который будет добавлен на втором шаге

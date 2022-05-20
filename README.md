<!DOCTYPE html>
<html lang="en" data-color-mode="auto" data-light-theme="light" data-dark-theme="dark" data-a11y-animated-images="system">
  <head>
    <meta charset="utf-8">
<h3 dir="auto" align="center">Спринт 10. Командная разработка проекта YaMDb.</h3>
<h3 dir="auto"><a id="user-content-описание" class="anchor" aria-hidden="true" href="#описание"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Описание</h3>
<p dir="auto">Проект YaMDb собирает отзывы пользователей на произведения. Произведения разделяются на категории. Список категорий может быть расширен администратором. Произведению может быть присвоен жанр. Сами произведения в YaMDb не хранятся, здесь нельзя посмотреть фильм или послушать музыку.Благодарные или возмущённые пользователи оставляют к произведениям текстовые отзывы (Review) и ставят произведению оценку в диапазоне от одного до десяти (целое число); из пользовательских оценок формируется усреднённая оценка произведения — рейтинг (целое число). На одно произведение пользователь может оставить только один отзыв.</p>
<h4 dir="auto"><a id="user-content-инструкция-по-развёртыванию" class="anchor" aria-hidden="true" href="#инструкция-по-развёртыванию"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Инструкция по установке проекта</h4>
<ul dir="auto">
<li>Произвести клонирование репозитория и перейти в его директорию:</li>
</ul>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="git clone https://github.com/Spektrogen/api_yamdb.git"><pre><span class="pl-s1">git</span> <span class="pl-s1">clone</span> <span class="pl-s1">https</span>:<span class="pl-s1">//</span><span class="pl-s1">github</span>.<span class="pl-s1">com</span><span class="pl-s1">/</span><span class="pl-s1">Spektrogen</span><span class="pl-s1">/</span><span class="pl-s1">api_yamdb</span>.<span class="pl-s1">git</span></pre></div>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="cd api_yamdb"><pre><span class="pl-s1">cd</span> <span class="pl-s1">api_yamdb</span></pre></div>
<ul dir="auto">
<li>Cоздать и активировать виртуальное окружение:</li>
</ul>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="python -m venv env"><pre><span class="pl-s1">python</span> <span class="pl-c1">-</span><span class="pl-s1">m</span> <span class="pl-s1">venv</span> <span class="pl-s1">env</span></pre></div>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="source venv/Scripts/activate"><pre><span class="pl-s1">source</span> <span class="pl-s1">venv</span><span class="pl-s1">/</span><span class="pl-s1">Scripts</span><span class="pl-s1">/</span><span class="pl-s1">activate</span></pre></div>
<ul dir="auto">
<li>Обновить pip, установить зависимости из requirements.txt</li>
</ul>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="python -m pip install --upgrade pip"><pre><span class="pl-s1">python</span> <span class="pl-c1">-</span><span class="pl-s1">m</span> <span class="pl-s1">pip</span> <span class="pl-s1">install</span> <span class="pl-c1">-</span><span class="pl-c1">-</span><span class="pl-s1">upgrade</span> <span class="pl-s1">pip</span></pre></div>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="pip install -r requirements.txt"><pre><span class="pl-s1">pip</span> <span class="pl-s1">install</span> <span class="pl-s1">-</span><span class="pl-s1">r</span> <span class="pl-s1">requirements</span>.<span class="pl-s1">txt</span></pre></div>
<ul dir="auto">
<li>Запустить сервер</li>
</ul>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" data-snippet-clipboard-copy-content="python manage.py runserver"><pre><span class="pl-s1">python</span> <span class="pl-s1">manage</span>.<span class="pl-s1">py</span> <span class="pl-s1">runserver</span></pre></div>
<h4 dir="auto"><a id="user-content-язык" class="anchor" aria-hidden="true" href="#язык"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Язык</h4>
<ul dir="auto">
<li>Python</li>
</ul>
<h4 dir="auto"><a id="user-content-стек-технологий" class="anchor" aria-hidden="true" href="#стек-технологий"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>В проекте использованы технологии</h4>
<ul dir="auto">
<li>Python</li>
<li>Django</li>
<li>Django REST Framework</li>
<li>Git</li>
</ul>
<h3 dir="auto"><a id="user-content-создатели-проекта" class="anchor" aria-hidden="true" href="#создатели-проекта"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Данный проект был создан</h3>
<ul dir="auto">
<li>Илья Мазанов</li>
<li>Никита Колпаков</li>
<li>Чувычкин Сергей</li>
</ul>
</article>
  </div>

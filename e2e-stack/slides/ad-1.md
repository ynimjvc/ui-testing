[Назад](/e2e-stack/slides/19.md)

---

# DOM

### Ноды

```html
<div id="foo">
    Text
    <div class="bar"
         data="fizz">
        special
        <br>
        text
    </div>
</div>
```

    `div` - нода с 2 дочерней нодой
    `text` - текстовая нода без дочерних элементов

---

### Селекторы

```html
<div id="foo"
     class="bar fizz">
    Text
    <div class="bar"
         data="fizz">
        special
        <br>
        text
    </div>
</div>
```

`div` - выберет все ноды с тегом `div`

`#foo` - выберет ноду с `id="foo"`

`.bar` - выберет ноды с классом `bar`

`.bar.fizz` - веберет ноды у которых есть оба класса `fizz` и `bar`

`.bar div` - веберт все ноды `div` которые являются потомками нод с классом `bar`

`.bar > div` - веберт все ноды `div` которые являются прямыми потомками нод с классом `bar`

`:first-child`, `:last-child`, `:nth-child(kn+m)` - выберут соответсвенно ноды которые являются
первым дочерним, последним или или удовлевлетворяют условию `kn+m`

`[data="fizz"]` - выберет ноды со значением атрибута `data` равным `fizz`

---

[Далее](/e2e-stack/slides/ad-2.md)

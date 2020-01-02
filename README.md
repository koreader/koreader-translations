# KOReader Translations

The translations for KOReader are collected in this repository. You can most easily contribute and collaborate through [the KOReader project on Weblate][koreader-weblate]. If you prefer you can also fork the repository and use your own tools, such as [Lokalize](https://userbase.kde.org/Lokalize) or [Virtaal](https://virtaal.translatehouse.org/). If you choose to do so, please try to submit your PR as soon as possible to prevent duplicate translation efforts.

Thanks to hosted Weblate, we profit from a translation memory shared with various other projects. [MyMemory](https://mymemory.translated.net/) can also be a good source of inspiration.

To update this submodule with the latest translations, you can use the following command in the main repository:

```
make po
```

If your language is not listed on the Weblate project, please don't hesitate
to send a language request [here][koreader-weblate].

## Variables in translation

Some strings contain variables that should remain unaltered in translation. These take the form of a `%` followed by a number from `1-99`, although you'll seldom see more than about 5 in practice. Please don't put any spaces between the `%` and its number. `%1` should always remain `%1`.
For example:

```lua
The title of the book is %1 and its author is %2.
```

This might be displayed as:

```lua
The title of the book is The Republic and its author is Plato.
```

To aid localization the variables may be freely positioned:

```lua
De auteur van het boek is %2 en de titel is %1.
```

That would result in:

```lua
De auteur van het boek is Plato en de titel is The Republic.
```

## Translation status

<a href="https://hosted.weblate.org/engage/koreader/?utm_source=widget">
<img src="https://hosted.weblate.org/widgets/koreader/-/koreader/multi-auto.svg" alt="Translation status" />
</a>

[koreader-weblate]:https://hosted.weblate.org/engage/koreader/

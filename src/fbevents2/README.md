# fbevents2

> makes it possible insert two Facebook pixels in a web page

If you have a web page with a Facebook pixel, you cannot insert another one. It will complain with a warning.

1. Replace `fbq` with `fbq2` in your second pixel tag
2. Download *fbevents.js* script, rename it to *fbevents2.js* and replace `fpq` with `fbq2` in its content too.
3. Host it somewhere with https, for instance, put it in the *gh-pages/assets/js/* folder in this repo.
4. Change the URL in your second pixel tag, pointing to the URL serving the *fbevents2.js* script, for instance replace

```
document,'script','//connect.facebook.net/en_US/fbevents.js');
```

with

```
document,'script','//be-media.github.io/js/fbevents2.js');
```

Now you can use the second pixel tag without problems.

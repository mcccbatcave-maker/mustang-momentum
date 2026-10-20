[README.md](https://github.com/user-attachments/files/33728819/README.md)
# Mustang Momentum

An interactive accessibility practice for Mercer County Community College faculty, from MercerOnline.
It has eight challenges, sixteen scored decisions, hands-on "experience the barrier" demos, badges and a printable action plan.

## Files

```
index.html                  The whole game (HTML, CSS and JavaScript in one file)
assets/mercer-logo.png      Mercer County Community College logo
assets/merceronline-logo.png  MercerOnline logo
assets/maverick.svg         Maverick the Mustang (original illustration; you can replace it with official mascot art)
```

## Publish on GitHub Pages

1. Create a repository (for example, `mustang-momentum`) and upload all of these files. Keep the `assets` folder.
2. In the repository, go to **Settings › Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, and save.
4. After a minute or two, the site is live at `https://<your-account>.github.io/mustang-momentum/`.
5. Link to that address from Blackboard, opening in a new tab.

## Customize

Near the top of the `<script>` in `index.html`:

- `CONFIG.supportUrl`: add a MercerOnline support page link. It appears in the Resources panel.
- `CONFIG.storageKey`: change this if you release a new version with different questions, so old saved progress resets cleanly.

All challenge text, questions and explanations are in the `CH` array in `index.html`.

To use official mascot artwork, replace `assets/maverick.svg` with a file of the same name. A square PNG also works if you update the `MAV` constant.

## Notes

- Progress is saved in the learner's browser (localStorage) only. Nothing is sent to Blackboard or to a server.
- Fonts (Montserrat and Atkinson Hyperlegible) load from Google Fonts. If they're blocked, system fonts are used instead.
- Two demos show barriers on purpose: pale-gold text in Challenge 5 and a mouse-only drag activity in Challenge 8. Both are labeled, both include an accessible equivalent, and neither is needed to finish the challenge.

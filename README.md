# Modellierung-Untertitel

Suggest changes per pull requests, please.

Note that the *editor settings* provided as an `.editorconfig` file can be enforced by most editors either [directly](https://editorconfig.org/#pre-installed) or [after installing some plugin](https://editorconfig.org/#download).

Some initial ideas for pull requests:

- Try to fix some spelling mistakes found by the bot, as in [this comment](https://github.com/fmidue/Modellierung-Untertitel/commit/a1bdf2392bf28dd614fe681e78bacd6fb8542c85#commitcomment-127307836).
- Annotate the beginnings of individual slides in the respective subtitle files as in [this commit](https://github.com/fmidue/Modellierung-Untertitel/commit/dfb9c2b63c722214f646214c67f87ac16152dce0). (Even though later videos don't have embedded slide numbers, the slides themselves, over at https://fmidue.github.io/Modellierung-Folien/, do indeed have numbers that can be referenced meaningfully. While adding slide numbers, make sure that the numbers are increasing per file, i.e., so that subsequent changes like in [this commit](https://github.com/fmidue/Modellierung-Untertitel/commit/45471cc49f6264219cd92347c0a262a8e986d2dd) do not become necessary.)
- Use ChatGPT to improve German and English grammar. For example, the changes in [this commit](https://github.com/fmidue/Modellierung-Untertitel/commit/c39be32e841ca33c43393868208aa54005280f06) were produced using the prompts
  > Bitte korrigiere Grammatikfehler in den folgenden Untertiteln. Aendere keine Zeilenumbrueche. Aendere nicht die Zuordnung von Zeitstempeln. Wenn die Grammatik korrekt ist, gib die vorgegebenen Untertitel genau so zurueck, wie sie sind. Hier sind die vorgegebenen Untertitel: ...

  and
  > Please correct grammar mistakes in the following subtitles. Do not change line breaks. Do not change the assignment of time stamps. If the grammar is correct, return the given subtitles exactly as they are. Here are the given subtitles: ...

  respectively. (But blindly taking over ChatGPT-produced changes will not work satisfactorily. Instead, going through them individually, and selecting the appropriate line changes, will most likely be necessary. Maybe use a tool like [Beyond Compare](https://www.beyondcompare.de/) or hunk staging with `git add -p` to facilitate this.)

## Leader board

| GitHub username | Lines |
| :-- | --: |
| timmycodesforfun | 72 |
| sabinxh | 7 |

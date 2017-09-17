# listen
Interactive Memo WebApp with Speech Recognition

## [Demo](https://dplusic.github.io/listen/)

## Notes
* Speech Recognition works on localhost or via https.
* Mobile browsers are also supported.

## References

### Speech Recognition
* [Annyang](https://www.talater.com/annyang/)
  * [Issue] [(Android) Repeated microphone notification](https://github.com/TalAter/annyang/issues/194)
    * Because of this issue, I tried to adopt `pocketsphinx.js` for keyword spotting on mobile browsers.
* [Pocketsphinx.js](https://syl22-00.github.io/pocketsphinx.js/)
  * [Issue] [PocketSphinx + Google SpeechRecognition + Android = NO](https://github.com/syl22-00/pocketsphinx.js/issues/51)
    * Solved by stopping an audio stream.
  * [Issue] [False detection when there is no audio](https://github.com/syl22-00/pocketsphinx.js/issues/60)
    * Because of this issue, I adopted `JsSpeechRecognizer` for keyword spotting on all browsers.
* [JsSpeechRecognizer](https://github.com/dplusic/JsSpeechRecognizer)
* [Chrome Web Speech API](https://developers.google.com/web/updates/2013/01/Voice-Driven-Web-Apps-Introduction-to-the-Web-Speech-API)

### Speech Synthesis
* [Chrome Speech Synthesis API](https://developers.google.com/web/updates/2014/01/Web-apps-that-talk-Introduction-to-the-Speech-Synthesis-API)

### Trigger
* [IFTTT Webhooks](https://ifttt.com/maker_webhooks)

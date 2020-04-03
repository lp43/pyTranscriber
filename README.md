# pyTranscriber

pyTranscriber是一款通過友善的圖形化界面為音頻/視頻文件生成 <b>語音轉文字/自動產生字幕</b> 的應用程式。語音識別的工作是用 <a href="https://cloud.google.com/speech/">Google Speech Recognition API (語音識別)</a> 以及 <a href="https://github.com/agermanidis/autosub">Autosub (自動生成字幕)</a> 來完成。<br>
![pyTranscriber1](doc/screenshot3.png?raw=true "pyTranscriber")
<br>
<br>
pyTranscriber 是作者前一個專案 <a href="https://github.com/raryelcostasouza/JAutosub">JAutosub (Java)</a> 的優化版本，created because of the limitations, issues, and overhead of mixing this 2 different languages on a single project.
<br>
<br>這款程式在預設狀況下，產出.srt的字幕檔與.txt的音頻辨識文字檔。SRT字幕檔可用 <a href="http://www.aegisub.org/">Aegisub</a> 進行編輯。
如同 <a href="https://support.google.com/youtube/answer/6373554?hl=en">Youtube Automatic Subtitles</a> 自動產生字幕技術，這款應用程式因為使用 <a href="https://cloud.google.com/speech/">Google Cloud Speech Server</a> 完成辨識工作，因此 **需要** 網路連線。
<br>
<br>重要提示：由於語音辨識技術尚未純熟，因此辨識的 <b>準確率</b> 皆不同，具體取決於許多因素，主要是音頻的 <b>音質/清晰度</b>。在理想情況下，音源不應有背景噪音、其它聲音效果或音樂。如果只有一個人在說話，並且他說話的速度清晰且緩慢，辨識則會更加精確。有時，在理想/幸運的狀況底下，甚至可以得到 <a href="https://medium.com/@mlockrey/youtube-s-incredible-95-accuracy-rate-on-auto-generated-captions-b059924765d5">近乎95%的精準度</a>。
<br>
<br>
![pyTranscriber2](doc/screenshot2.png?raw=true "pyTranscriber")
![pyTranscriber3](doc/screenshot1.png?raw=true "pyTranscriber")
<br>
<br>

<h1>Release Notes:</h1>
<b>2020/04/03 - v1.4.1:</b>
<br>* 將音頻辨識預設為繁體中文
<br><b>2020/01/29 - v1.4:</b>
<br>* Fixed crash when exporting txt file for languages with special characters, specially chinese, on Windows system. Thanks for KY Poon for reporting!
<br><br>
<b>2019/10/18 - v1.3:</b>
<br>* Added option for not opening output transcription files automatically after finish
<br>* Fixed bug with canceling during batch processing (only the current job was being stopped... not all of them as expected).
<br><br>

<h1>給使用者 - 下載 Windows/Linux/MacOS portable app</h1>

<a href="https://github.com/raryelcostasouza/pyTranscriber/releases/tag/v1.4-stable"> pyTranscriber-v1.4-stable</a>

<h1>給開發者 - 技術文件</h1>

Check at <a href="https://github.com/raryelcostasouza/pyTranscriber/blob/master/doc/technical_details.md">technical_details.md<a>

### License

GPL v3

# BEAT / TYPE

Audio-reactive typography editor / 音频响应文字编辑器。

## Included / 已包含
- Music: audio level animation and peak-triggered line changes (not BPM tracking).
- Speech: continuous volume response and adjustable silence-triggered line changes.
- Demo audio, uploaded audio, microphone, voice recording, browser-supported video export.
- Input meter, silence diagnostics and interrupted-audio resume control.

音乐按声音峰值换句；人声按停顿换句。两者都不做语音转写或逐字对齐。

## Run / 运行
Serve the dist folder through localhost or HTTPS. For example, with Python 3 installed:

    python3 -m http.server 8000 --directory dist

Open http://localhost:8000 . Microphone access requires browser permission.

## Validation / 验证
JavaScript syntax and simulated PCM tests passed for low-volume response, recording-time animation, silence decay, pause switching, initial/extended silence, final-line hold, mode separation and music regression. Real microphone, Safari recording and exports still require device testing.

## Status / 状态
This export includes the prepared Music/Speech update that is not yet deployed to the existing Sites URL. GitHub synchronization does not itself deploy the app.

## Still planned / 未实现
Actual BPM tracking, video audio extraction UI, SRT export, speech recognition/word alignment, transparent animation export and editor integration.

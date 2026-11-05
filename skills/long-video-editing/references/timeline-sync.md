[English](#english) · [简体中文](#简体中文)

## English

# Timeline synchronization after speech changes

Use when inserting, deleting, reordering speech, or replacing voiceover in an existing project. Read current state before editing. Preserve approved structure, media, styles, and manual positions. If the user is still editing speech, prepare media/scripts/styles without binding all overlays to stale timing; reread after they finish.

## Edit content through the transcript

In ChatCut, use the current speech-editing / Script workflow to select, copy, delete, and reorder original utterances. Fix caption/transcript text through the appropriate text correction workflow. Do not replace script-led editing with timestamp searches and manual slicing.

- Change only the target speech track. Returned transcripts may include other tracks; inspect scope before submitting so a small edit does not reorder unrelated content.
- Preserve non-transcribable transitions, non-speech clips, necessary gaps, and existing cuts. If exact existing timing matters, read a representation including silence/non-transcribed segments.
- Copy source transcript items for new sentences from footage; do not fabricate unspoken lines by changing text.
- Preview the plan. Compare added/retained clips, total duration, source content, and order. If a small change removes transitions or alters large portions, correct the plan before submitting.
- For copying, verify the new opening playback and the original sentence still in the body, not just one occurrence.
- Reread actual placements after submission. Use the real frame rate, preserving non-integer rates and distinguishing seconds from frames.

## Synchronize all dependent layers

Use semantic/source mappings before and after the change to align:

- Chapter headings, quotes, questions, term annotations, and lists.
- Screenshots, demos, profile images, and speaker insets.
- Persistent identities and their visibility during shot changes.
- Separate voiceovers, audio, and muted video duplicates.
- Captions, chapter bar, its internal chapter start times, and total duration.
- Opening transition, final introduction, and series purpose.
- Delivered publishing timestamps and topic entries; recheck source frames when a cover is requested from a final-cut time.

Single-track ripple behavior does not necessarily synchronize other tracks. Multiple cuts and frame-rounding differences also prevent applying one uniform offset to everything. Establish mappings from current clip boundaries and check semantic anchors.

Persistent items crossing an insertion may need extending; following text may need shifting; new speech needs its own visuals rather than the next sentence's overlay. Preserve established same-type size, position, and background style.

Speech editing may remove previous seam treatment. After structure stabilizes, add brief audio crossfades or gentle fades where affected, preserving natural syllables without conspicuous visual transitions.

## Captions & audio

Refresh captions in edit order, retaining corrected names, terminology, and sparse manual edits. Do not unnecessarily overwrite user caption styles.

At clip boundaries, check whether words from the next sentence leaked in. Fix caption cards for zero-duration/display issues; tighten the content edit when audio actually contains the next sentence. Deleting a subtitle cannot hide an audio cut error.

New copied clips inherit existing noise cleanup, volume, and color treatment. Align replacement voiceover using actual meaning, speech onset, and ending, checking both duration and content.

## Minimum verification

Check before insertion, during inserted speech, return to the original, transition, first affected chapter, a distant chapter, and the last frame. Verify retained original sentence, caption text, voiceover position, and navigation length.

Inspect composed pixels and available audio or comparisons for seams. If only saved data can be confirmed, state the missing playback/listening check; tool success is not correct playback.

Update delivered show notes/timestamps using current topic entries after edits. Do not use old script times or assume one offset for the entire video. See [Publishing materials](publishing.md).

---

## 简体中文

# 改稿后的时间线同步

用于已铺字幕和素材的项目：插句、删句、复制钩子、调序、替换音频，以及用户手动剪辑后的重新对齐。

## 先刷新，再改

读取当前项目、目标时间线、受影响的口播片段和其他轨道，不使用上次回复中的旧时间点。记录帧率、原长度、相关片段起止和用户手调样式；较大重排保留可恢复版本或轻量修改记录。

如果用户还在手动剪口播，先做素材、文稿和样式，不把所有叠层绑死在旧时间线。收到“口播剪完”后再读取最新顺序和时间。

## 内容修改走文字剪辑

在 ChatCut 中，按当前环境的语音剪辑／Script 工作流选择原话、复制、删除和调序；字幕修正走字幕或转写修正工作流。不要用查时间戳再手动切片代替基于文稿的内容剪辑。

- 只修改目标语音轨。返回的文稿可能含其他轨道，提交前检查作用范围，不让一次小改重排无关轨道。
- 保留不可转写的过渡画面、非语音片段、必要空隙和原有剪口。需要精确保留现有时序时，读取包括静音／非转写片段的完整表示。
- 对原片引入的新句，复制相应源文稿条目；不要改文字来伪造没说过的句子。
- 先预览编辑计划。比较新增和保留的片段、总时长、源内容与顺序；如果一个小改意外删掉过渡或改变大段原剪辑，修正计划后再提交。
- 用户要求复制时，既验证开头的新播放，也验证正文仍覆盖原句，不能仅检查是否出现过一次。
- 提交后重新读取实际落点。帧率取实际值，不能把非整数帧率按整数处理，也不能把秒和帧混用。

## 联动全部依赖层

依实际修改前后的语义／源片映射，对齐以下内容：

- 章节标题、金句、问题、术语注释和列举文字。
- 截图、演示素材、资料照片和单人小窗。
- 常驻人物介绍及切镜时的显示区间。
- 独立旁白、音频、静音画面副本。
- 字幕、底部章节条及其内部保存的各章节起点和总片长。
- 开头过渡、最后自我介绍与栏目发心。
- 已经制作的发布章节时间轴及其话题入口；用户指定成片某一时刻做封面时，也重新核对它对应的源画面。

单轨自动吸附或波纹剪辑不会天然同步其他轨道；一个项目有多个剪点或帧舍入差异时，也不能只对所有素材机械加同一个秒数。用当前片段边界建立对应关系，再核对关键语义锚点。

跨越插入点的常驻元素可能需要延长；紧跟插入点出现的文字应后移；针对新句的画面不能沿用下一句的花字。原来属于同类样式的字号、位置和底色应保留。

语音剪辑可能移除原有接音处理。最终结构稳定后，为受影响语音做短音频交叉衔接或轻微淡入淡出；保留自然音节，不添加显著视觉转场。

## 字幕和音频的特殊检查

刷新剪辑后的字幕，并保留已校对的姓名、术语和稀疏手动修改。不要为重排而无必要地覆盖用户字幕样式。

检查片段边界处是否把下一句的字带进字幕。若只是零时长词或显示边界问题，修字幕卡；若实际音频带入下一句，则回到文字剪辑收紧内容边界，不靠删字幕掩盖音频。

新复制片段继承整片已有的降噪、音量和色彩处理。替换旁白后按实际内容、开口时间和结束时间对齐画面，既检查时长也检查意思。

## 最小验收

检查插入点之前、插入句中、接回原句后、过渡、首个受影响章节、远端一个章节和最后一帧。再核对原句保留、字幕文字、旁白位置、章节导航总长度。

查看实际合成像素；需要判断接音时查看可用的音频或前后对比。只能确认数据保存时，明确说明未能试听或预览，不把工具返回成功当作播放已正确。

如果 shownote 或发布时间轴已经交付，剪辑变化后按最新话题入口重新生成受影响时间点，不沿用旧文稿时间，也不假设全片只需统一增加一个秒数。相关方法见 [封面与发布素材](publishing.md)。

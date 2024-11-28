<script lang="ts">
	import { browser } from "$app/environment";

    const tweets = [
        {
            title: 'イベント概要',
            contents: '<blockquote class="twitter-tweet"><p lang="ja" dir="ltr">🌺お知らせ🌺<br><br>12月1日(日) 19:00-<br><br>「HibiscusCUP ver_Gunfight」<br><br>　　開催決定！！🥳🎉<br><br>第3回でご好評頂いた<br>「エネミーフラッグ戦」のみを行う<br>銃撃戦メインのイベントです！<br><br>今回も視聴者プレゼントあり！<br>どのチームを応援する？<br><br>お楽しみに！🌺 <a href="https://t.co/h6ffan1wD7">pic.twitter.com/h6ffan1wD7</a></p>&mdash; りえぺこ🌺:) タルコフイベ12/1開催 (@Riepeko_yolo) <a href="https://twitter.com/Riepeko_yolo/status/1857710327695118537?ref_src=twsrc%5Etfw">November 16, 2024</a></blockquote>'
        },
        {
            title: 'プレゼント企画',
            contents: '<blockquote class="twitter-tweet"><p lang="ja" dir="ltr">🌺HibiscusCUP🌺<br><br>\視聴者プレゼントキャンペーン！/<br><br>「<a href="https://twitter.com/hashtag/HibiscusCUP?src=hash&amp;ref_src=twsrc%5Etfw">#HibiscusCUP</a>」 と<br>「応援チームA.B.Cいづれか」<br>を記入して応援をポストしよう！<br><br>ゆんま先生(<a href="https://twitter.com/Yuika_flw?ref_src=twsrc%5Etfw">@Yuika_flw</a>)が描く<br>優勝チームイラスト、大会ロゴ等<br>ゆんま工房オリジナル缶バッジが当たる！<br><br>※住所を教えて頂ける方<br>当選者数：３名… <a href="https://t.co/XxuyEdKKLx">https://t.co/XxuyEdKKLx</a> <a href="https://t.co/WFKnE95Zix">pic.twitter.com/WFKnE95Zix</a></p>&mdash; りえぺこ🌺:) タルコフイベ12/1開催 (@Riepeko_yolo) <a href="https://twitter.com/Riepeko_yolo/status/1860609305243787733?ref_src=twsrc%5Etfw">November 24, 2024</a></blockquote>'
        },
    ];
</script>

<div>
    {#if browser}
        <script async src="https://platform.twitter.com/widgets.js"></script>
    {/if}

    {#each tweets as tweet}
    <div class="text-center flex justify-center">
        <div>
            {@html tweet.contents}
        </div>
    </div>
    {/each}
</div>

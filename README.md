# -<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>乃木坂46 CD形態比較ナビ</title>
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            nogi: '#742581',
            nogiLight: '#9b3fa8',
            nogiBg: '#f8f1fa'
          }
        }
      }
    }
  </script>
</head>
<body class="bg-slate-50 text-slate-800 min-h-screen">

  <!-- ヘッダー -->
  <header class="bg-nogi text-white py-6 px-4 shadow-md text-center">
    <div class="inline-block bg-white/20 text-white text-[11px] font-bold px-2.5 py-0.5 rounded-full mb-1">
      2026年9月最新版 / 6期生対応
    </div>
    <h1 class="text-2xl font-bold tracking-tight">乃木坂46 CD形態別比較ナビ</h1>
    <p class="text-xs text-purple-200 mt-1">「推しの曲・映像がどのTypeに入っているか」すぐわかる比較表</p>
  </header>

  <main class="max-w-6xl mx-auto px-4 py-6">
    
    <!-- 絞り込みコントロールバー -->
    <div class="bg-white rounded-2xl shadow-sm p-4 mb-6 border border-slate-200 flex flex-col md:flex-row gap-4 items-center justify-between">
      
      <!-- シングル切り替え -->
      <div class="w-full md:w-auto flex items-center gap-2">
        <label for="singleSelect" class="text-xs font-bold text-slate-500 whitespace-nowrap">作品選択:</label>
        <select id="singleSelect" class="w-full md:w-64 border border-slate-300 rounded-lg px-3 py-2 text-sm font-semibold focus:outline-none focus:ring-2 focus:ring-nogi bg-slate-50">
          <option value="42">42nd『是非に及ばず』(2026.07)</option>
          <option value="41">41st『最後に階段を駆け上がったのはいつだ？』(2026.04)</option>
          <option value="40">40th『ビリヤニ』(2025.11)</option>
        </select>
      </div>

      <!-- 推しメン選択 -->
      <div class="w-full md:w-auto flex items-center gap-2">
        <label for="memberFilter" class="text-xs font-bold text-slate-500 whitespace-nowrap">推しメン:</label>
        <select id="memberFilter" class="w-full md:w-64 border border-slate-300 rounded-lg px-3 py-2 text-sm font-semibold focus:outline-none focus:ring-2 focus:ring-nogi bg-white">
          <option value="">全員表示（選択解除）</option>
          
          <optgroup label="3期生">
            <option value="伊藤理々杏">伊藤理々杏</option>
            <option value="岩本蓮加">岩本蓮加</option>
          </optgroup>

          <optgroup label="4期生">
            <option value="遠藤さくら">遠藤さくら</option>
            <option value="賀喜遥香">賀喜遥香</option>
            <option value="金川紗耶">金川紗耶</option>
            <option value="黒見明香">黒見明香</option>
            <option value="柴田柚菜">柴田柚菜</option>
            <option value="田村真佑">田村真佑</option>
            <option value="筒井あやめ">筒井あやめ</option>
            <option value="林瑠奈">林瑠奈</option>
            <option value="弓木奈於">弓木奈於</option>
          </optgroup>

          <optgroup label="5期生">
            <option value="五百城茉央">五百城茉央</option>
            <option value="池田瑛紗">池田瑛紗</option>
            <option value="一ノ瀬美空">一ノ瀬美空</option>
            <option value="井上和">井上和</option>
            <option value="岡本姫奈">岡本姫奈</option>
            <option value="小川彩">小川彩</option>
            <option value="奥田いろは">奥田いろは</option>
            <option value="川﨑桜">川﨑桜</option>
            <option value="菅原咲月">菅原咲月</option>
            <option value="冨里奈央">冨里奈央</option>
            <option value="中西アルノ">中西アルノ</option>
          </optgroup>

          <optgroup label="6期生">
            <option value="愛宕心響">愛宕心響</option>
            <option value="大越ひなの">大越ひなの</option>
            <option value="小津玲奈">小津玲奈</option>
            <option value="海邉朱莉">海邉朱莉</option>
            <option value="川端晃菜">川端晃菜</option>
            <option value="鈴木佑捺">鈴木佑捺</option>
            <option value="瀬戸口心月">瀬戸口心月</option>
            <option

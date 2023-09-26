<template>
  <div class="w-full">
    <CommonHeader>
      帮助
    </CommonHeader>

    <InstallPwa />

    <FeedbackActions />

    <div class="mx-auto max-w-md w-full rounded-2xl p-2" text-left>
      <FAQItem title="未来计划？">
        计划增加新功能，如自定义菜谱，与使用其他用户分享的菜谱。
      </FAQItem>

      <FAQItem title="什么是模式？">
        <ul>
          <li><b>模糊匹配</b>：展示所有含当前选中任意食材的菜谱</li>
          <li><b>精准匹配</b>：展示所有含当前选中所有食材的菜谱</li>
          <li><b>生存模式</b>：展示当前选中食材即可制作的所有菜谱</li>
        </ul>
      </FAQItem>

      <FAQItem title="如何快速清空所选食材和工具?">
        <div inline-flex items-center justify-center>
          点击顶部 <div i-mdi-pot-steam-outline mx-1 inline-block /> 图标即可。
        </div>
      </FAQItem>

      <FAQItem title="是否有 APP?">
        <b>暂时没有开发 APP 的计划。</b>
        但我们正在优化 <b>PWA</b> 的体验，以便您可以直接将本站添加到桌面，并享受<b>类似 APP 的体验</b>。
        <br>
        你可以使用浏览器打开，点击上方的<b>「安装到桌面」</b>或在菜单中点击<b>「添加到主屏幕」</b>。
      </FAQItem>

      <FAQItem title="未来是否会收费？">
        该项目将以免费开源的形式运营。
        <br>
      </FAQItem>

      <FAQItem title="页面无法点击、资源加载失败？">
        <blockquote>
          试试「无痕模式」是否正常？
        </blockquote>
        <br>
        <ol>
          <li>
            <b>清除 Cookie</b>
            <ol>
              <li>
                点击浏览器网址前方的 🔒 图标
              </li>
              <li>
                点击「Cookie」并清除
              </li>
            </ol>
          </li>
          <li>
            <b>强制刷新缓存</b>
            <ul>
              <li>Windows: <code>Ctrl + F5</code></li>
              <li>macOS: <code>Cmd + Shift + R</code></li>
            </ul>
          </li>
        </ol>
      </FAQItem>

      <hr h="1" my="4" bg-black>

      <FAQItem :default-open="true" title="关于">
        <div text-left>
          <ul>
            <li>
              它诞生于 2022 年 4 月，时值疫情风控期间，希望能帮助期间的伙伴根据现有食材寻找到合适的菜谱。故原名「隔离食用手册」。
            </li>
            <li>
              如今那个时期已离我们远去，故去掉「隔离」二字。但也很高兴能在这里继续与你相遇，希望它能继续发光发热，在日常生活中帮助到大家。
            </li>
            <li>
              <div class="inline-flex items-center justify-center">
                代码仓库：<a class="inline-flex items-center justify-center" href="https://github.com/YunYouJun/cook" target="_blank">
                  <div m="r-1" i-ri-github-line inline-flex />YunYouJun/cook</a>
              </div>
            </li>
            <li>
              <div class="inline-flex items-center justify-center">
                菜谱视频来源：
                <a class="inline-flex items-center text-sm text-blue-600 dark:text-blue-400" href="https://docs.qq.com/sheet/DQk1vdkhFV0twQVNS" target="_blank">
                  <div m="r-1" i-ri-bilibili-line inline-flex />
                  <span class="inline-flex">隔离食用手册大全</span>
                </a>
              </div>
            </li>
          </ul>
        </div>
      </FAQItem>
    </div>
  </div>
  <BaseFooter mt-4 />
</template>

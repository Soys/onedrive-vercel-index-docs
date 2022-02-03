# 有何新特性？

🎉 这里是一个包含本项目新特性而不断更新的页面。也可从在 [What's new? #325](https://github.com/spencerwooo/onedrive-vercel-index/discussions/325) 中查看。

#### 2022/2/2

- 🎥 我们放弃使用 `react-player` ，现在分别使用 `react-dplayer` 和 `react-audio-player` 作为视频播放器和音频播放器。
- 🎇 我们为视频增加了缩略图渲染，下方查看差别：

  |                                  使用前                                  |                                使用后                                |
  | :----------------------------------------------------------------------: | :-----------------------------------------------------------------: |
  | ![旧版本无缩略图渲染](./_images/old-no-thumbnail.png) | ![新版本缩略图渲染](./_images/new-with-thumbnail.png) |

- 💬 我们增加了对字幕(隐藏字幕)的支持，若有与视频同名的有效`.vtt`webvtt格式字幕文件存在，它将会被自动引用。

  |                                 使用前                                  |                                    使用后                                     |
  | :---------------------------------------------------------------------: | :--------------------------------------------------------------------------: |
  | ![旧版本不支持字幕](./_images/old-no-subtitle.png) | ![新版本尝试引用字幕](./_images/new-with-subtitle.png) |

- ⚡️ 为了更快的构建速度和更有效率的使用缓存，我们已经将项目的包管理器从`npm`迁移至`pnpm`。你可能需要更新你Vercel的构建命令：

  ![从 npm 迁移至 pnpm](./_images/pnpm-commands.png)

  - 构建命令： `pnpm build`
  - 安装命令： `pnpm install`

#### 2022/1/29

- ❗**重大更新** - 配置文件从`.json`变更至`.config.js`， 已添加相关注释。你现在可以将`userPrincipleName`移动到Vercel的环境变量（避免在公共场合暴露你的邮箱地址）。
- CORS头部现在存在于路径为`?raw=true`的OneDrive原始文件链接。

#### 2022/1/22

- 🔍 [Supporting search for all versions of OneDrive #295](https://github.com/spencerwooo/onedrive-vercel-index/discussions/295)

#### 2022/1/11

- 📚 [New documentation site live #264](https://github.com/spencerwooo/onedrive-vercel-index/discussions/264)

#### 2022/1/10

- 🚫 由于Vercel的限制，移除对代理下载的支持：[Proxied download not working - 无法使用代理下载 #251](https://github.com/spencerwooo/onedrive-vercel-index/discussions/251).

#### 2022/1/1

- 🚀 我们不再需要额外的部署tokens/secret设置：[New version update: No extra deployment setup is required anymore! #215](https://github.com/spencerwooo/onedrive-vercel-index/discussions/215)

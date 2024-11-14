# DWMBlurGlass

창 제목바에 커스텀 효과를 적용시키는 프로그램입니다. (윈도우 10, 11 지원)

给全局系统标题栏添加自定义效果，支持win10和win11
#
| [中文](/README_ZH.md) | [English](/README.md) | [italiano](/README_IT.md) | [français](/README_FR.md) | [Türkçe](/README_TR.md) | [español](/README_ES.md) | [German](/README_DE.md) | [한국어](/README_KO.md)

이 프로젝트는 [LGNU V3 라이센스](/COPYING.LESSER)를 사용합니다.

## !!! DWMBlurGlass는 다른 곳에서 다운로드 하지마세요!!!!
> [!WARNING]
> 저희는 누군가가 저희를 따라하는 것과 악성코드를 포함한 DWMBlurGlass를 배포하는 것을 발견했습니다.
> 
> 이 사태가 발생하는 걸 막기 위해서, 절대 이 소프트웨어를 비공식적인 곳에서 다운받지 마세요!
> 
> **저희는 또한 공식 디스코드 서버가 없습니다.**
> 
> 저희는 [Github](https://github.com/Maplespe/DWMBlurGlass/releases), [Bilibili](https://space.bilibili.com/87195798), [winmoes](https://winmoes.com)에서만 소프트웨어를 배포하고 있습니다.
> 
> 또한, 미리 배포하는 대신에, 테스트용 브랜치에서 먼저 새로운 버전을 올리고 있습니다.

[![라이센스](https://img.shields.io/github/license/Maplespe/DWMBlurGlass.svg)](https://www.gnu.org/licenses/lgpl-3.0.en.html)
[![Github 모든 버전](https://img.shields.io/github/downloads/Maplespe/DWMBlurGlass/total.svg)](https://github.com/Maplespe/DWMBlurGlass/releases)
[![최신 버전](https://img.shields.io/github/release/Maplespe/DWMBlurGlass.svg)](https://github.com/Maplespe/DWMBlurGlass/releases/latest)
<img src="https://img.shields.io/badge/language-c++-F34B7D.svg"/>
<img src="https://img.shields.io/github/last-commit/Maplespe/DWMBlurGlass.svg"/>  

## Catalog
- [효과](#효과)
- [호환성](#호환성)
- [갤러리](#갤러리)
- [이펙트 목록](#이펙트-목록)
  - [Blur](#blur)
  - [에어로](#aero)
  - [아크릴](#acrylic)
  - [Mica](#mica)
  - [MicaAlt](#micaalt)
- [사용하는 법](#how-to-use)
  - [설치](#install)
  - [삭제](#uninstall)
- [언어 파일들](#language-files)
- [디펜던시 파일들](#dependencies)

## 효과
* 커스텀 효과를 창 제목 바에다가 적용
* 조절할 수 있는 전체 투명화 범위 또는 제목 바 투명화 범위
* 조절할 수 있는 제목 바 색 혼합
* 조절할 수 있는 제목 바 색
* 에어로 리플렉션 및 패럴랙스 효과 이용 가능 
* 윈도우 7 형식 제목 바 버튼 높이 복구 가능
* 윈도우 7 API(DwmEnableBlurBehindWindow)를 사용하여 투명화 효과를 프로그램에 적용
* `Blur`, `에어로`, `아크릴`, `Mica(윈도우 11 전용)` 효과 지원
* 조절할 수 있는 각 자동 라이트/다크 모드 변경
* `CustomBlur`, `AccentBlur`, `SystemBackdrop` 의 투명화 방식 이용 가능
* 서드파티 테마 지원

![image](/Screenshot/001701.png)
![image](/Screenshot/10307.png)

## 호환성
최소 **윈도우 10 2004 버전** 부터 **최신 윈도우 11 버전** 까지 지원합니다. (몇몇 투명화 방식들은 윈도우 참가자 빌드에서 지원하지 않습니다.)

DWM을 더 커스텀마이징 하기 위해 서드 파티 테마랑 같이 쓰일 수 있습니다.

저희는 MicaForEveryone과의 방식과 다르게 소프트웨어의 렌더링 방식을 바꾸지 않기에 서드파티 프로그램 호환성을 최대화 시킵니다.

저희는 DWM을 역분석 하였고 굉장히 멋진 비주얼 효과들을 가져오기 위해 새로운 투명화 방식을 생성했습니다. 그러나 'SystemBackdrop' 투명화 방식을 고르면, 시스템의 이용 가능한 인터페이스를 사용하며 MicaForEveryone와 같은 효과를 가질 것입니다.

Not recommended for use with MicaForEveryone, we do not guarantee compatibility with it.
MicaForEveryone과 같이 쓰는건 추천하지 않습니다. 그 프로그램과의 호환성을 보장하지는 않습니다.

[ExplorerBlurMica](https://github.com/Maplespe/ExplorerBlurMica)와 호환됩니다. 같이 작동이 잘 됩니다.

[TranslucentFlyouts](https://github.com/ALTaleX531/TranslucentFlyouts)와 호환됩니다. (**TranslucentFlyouts와 이 프로젝트는 호환되지만, ExplorerBlurMica은 TranslucentFlyoutsV2와 호환되지 않는다는 걸 명심해야 합니다.**)
## 갤러리
<details><summary><b>Windows 11</b></summary>
  
![image](/Screenshot/10307.png)

![image](/Screenshot/102134.png)

> "Override DWMAPI mica effect (win11)" 활성화

![image](/Screenshot/013521.png)
</details>

<details><summary><b>Windows 10</b></summary>

![image](/Screenshot/001701.png)

![image](/Screenshot/100750.png)

서드 파티 테마

> "Extend effects to borders (win10)" 활성화

> "Aero reflection effect (win10)" 활성화

> "Reduce title bar button height (win7 style)" 활성화

![image](/Screenshot/025410.png)

</details>

## 이펙트 목록
### Blur
> Basic pure blur. Nothing special.

![image](/Screenshot/blur.png)

### Aero
> Windows 7's glass effect, with saturation and exposure effects on the background when a window is inactive.

![image](/Screenshot/aero.png)

![image](/Screenshot/aero_inactive.png)

### Acrylic
> The acrylic recipe: background, blur, exclusion blend, saturation, color/tint overlay and noise.

![image](/Screenshot/acrylic.png)

### Mica
> The Mica recipe: blurred wallpaper, saturation and color/tint overlay.

![image](/Screenshot/mica.png)

### MicaAlt
All of the above effects can be customized to blend colors.

MicaAlt is Mica with a grayish tone, you can modify the blend color by yourself to get the MicaAlt effect.

## How to use

### Install
1. Download the compiled program archive from the [Release](https://github.com/Maplespe/DWMBlurGlass/releases) page.
2. Unzip it to a location such as "`C:\Program Files`".
<details><summary><b>3. Run the DWMBlurGlass.exe GUI program and click Install.</b></summary>

![image](/Screenshot/012746.png)

>If nothing happens when you click Install, then you need to click on the Symbols page and click Download.

>**You may receive a notification about missing symbols in the future, especially after system updates.**

![image](/Screenshot/012924.png)

</details>

### Uninstall
1. Run the DWMBlurGlass.exe GUI program and click Uninstall.
2. Delete relevant files

## Language files
We offer several languages, such as English, Simplified Chinese, Spanish, Portuguese and more.
If you would like to help us translate into other languages, please see below for language file formats.

1. First, you need to fork this repository and clone it locally.
2. Open the "`Languagefiles`" folder and select an existing language such as "`en-US.xml`" and make a copy.
3. Rename the code to the name of the [target language](https://learn.microsoft.com/en-us/windows/win32/intl/locale-names) and open the xml file in your favorite text editor.
4. In the second line, in the "`local`" field, change it to your target language code, which should be the same as the filename (without the .xml extension).
5. You can put your name in the "`author`" field.
6. Next, please translate the field values in the xml format (be careful not to translate the field names) The correct format is:`<config>Config</config>` to `<config>xxxx</config>`.
7. Save your file when finished and copy it to the "data\lang" directory in the folder where the DWMBlurGlass.exe program is located.
8. Next, open DWMBlurGlass.exe and test the language file to see if it works correctly. If it doesn't, check the language code settings and check that the file conforms to the xml format specification.
9. Finally, commit the file to your own forked repository and send a pull request to the main branch of the project.
10. After the request is approved, your file will be released with a future software update.
   

## Dependencies
* MiaoUI interface library v2 (Private)
* [AcrylicEverywhere](https://github.com/ALTaleX531/AcrylicEverywhere) - Separate upstream implementation of the CustomBlur method, thanks to ALTaleX for research and support.
* [minhook](https://github.com/m417z/minhook)
* [pugixml](https://github.com/zeux/pugixml)
* [VC_LTL](https://github.com/Chuyu-Team/VC-LTL5)
* [Windows Implementation Libraries](https://github.com/Microsoft/wil)

Since the GUI program uses private libraries, only insiders can compile the GUI, which does not affect the compilation of the libraries.

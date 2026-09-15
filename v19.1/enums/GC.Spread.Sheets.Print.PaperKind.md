# Enumeration: PaperKind

[Sheets](../modules/GC.Spread.Sheets.md).[Print](../modules/GC.Spread.Sheets.Print.md).PaperKind

指定打印页面的纸张类型。

**`example`**
```javascript
activeSheet.setArray(0, 0, new Array(60).fill(["sample text"]));
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.paperSize(new GC.Spread.Sheets.Print.PaperSize(GC.Spread.Sheets.Print.PaperKind.a4));
activeSheet.printInfo(printInfo);
spread.print(0);
```

## Table of contents

### Enumeration members

- [a2](GC.Spread.Sheets.Print.PaperKind.md#a2)
- [a3](GC.Spread.Sheets.Print.PaperKind.md#a3)
- [a3Extra](GC.Spread.Sheets.Print.PaperKind.md#a3extra)
- [a3ExtraTransverse](GC.Spread.Sheets.Print.PaperKind.md#a3extratransverse)
- [a3Rotated](GC.Spread.Sheets.Print.PaperKind.md#a3rotated)
- [a3Transverse](GC.Spread.Sheets.Print.PaperKind.md#a3transverse)
- [a4](GC.Spread.Sheets.Print.PaperKind.md#a4)
- [a4Extra](GC.Spread.Sheets.Print.PaperKind.md#a4extra)
- [a4Plus](GC.Spread.Sheets.Print.PaperKind.md#a4plus)
- [a4Rotated](GC.Spread.Sheets.Print.PaperKind.md#a4rotated)
- [a4Small](GC.Spread.Sheets.Print.PaperKind.md#a4small)
- [a4Transverse](GC.Spread.Sheets.Print.PaperKind.md#a4transverse)
- [a5](GC.Spread.Sheets.Print.PaperKind.md#a5)
- [a5Extra](GC.Spread.Sheets.Print.PaperKind.md#a5extra)
- [a5Rotated](GC.Spread.Sheets.Print.PaperKind.md#a5rotated)
- [a5Transverse](GC.Spread.Sheets.Print.PaperKind.md#a5transverse)
- [a6](GC.Spread.Sheets.Print.PaperKind.md#a6)
- [a6Rotated](GC.Spread.Sheets.Print.PaperKind.md#a6rotated)
- [aPlus](GC.Spread.Sheets.Print.PaperKind.md#aplus)
- [b4](GC.Spread.Sheets.Print.PaperKind.md#b4)
- [b4Envelope](GC.Spread.Sheets.Print.PaperKind.md#b4envelope)
- [b4JisRotated](GC.Spread.Sheets.Print.PaperKind.md#b4jisrotated)
- [b5](GC.Spread.Sheets.Print.PaperKind.md#b5)
- [b5Envelope](GC.Spread.Sheets.Print.PaperKind.md#b5envelope)
- [b5Extra](GC.Spread.Sheets.Print.PaperKind.md#b5extra)
- [b5JisRotated](GC.Spread.Sheets.Print.PaperKind.md#b5jisrotated)
- [b5Transverse](GC.Spread.Sheets.Print.PaperKind.md#b5transverse)
- [b6Envelope](GC.Spread.Sheets.Print.PaperKind.md#b6envelope)
- [b6Jis](GC.Spread.Sheets.Print.PaperKind.md#b6jis)
- [b6JisRotated](GC.Spread.Sheets.Print.PaperKind.md#b6jisrotated)
- [bPlus](GC.Spread.Sheets.Print.PaperKind.md#bplus)
- [c3Envelope](GC.Spread.Sheets.Print.PaperKind.md#c3envelope)
- [c4Envelope](GC.Spread.Sheets.Print.PaperKind.md#c4envelope)
- [c5Envelope](GC.Spread.Sheets.Print.PaperKind.md#c5envelope)
- [c65Envelope](GC.Spread.Sheets.Print.PaperKind.md#c65envelope)
- [c6Envelope](GC.Spread.Sheets.Print.PaperKind.md#c6envelope)
- [cSheet](GC.Spread.Sheets.Print.PaperKind.md#csheet)
- [custom](GC.Spread.Sheets.Print.PaperKind.md#custom)
- [dSheet](GC.Spread.Sheets.Print.PaperKind.md#dsheet)
- [dlEnvelope](GC.Spread.Sheets.Print.PaperKind.md#dlenvelope)
- [eSheet](GC.Spread.Sheets.Print.PaperKind.md#esheet)
- [executive](GC.Spread.Sheets.Print.PaperKind.md#executive)
- [folio](GC.Spread.Sheets.Print.PaperKind.md#folio)
- [germanLegalFanfold](GC.Spread.Sheets.Print.PaperKind.md#germanlegalfanfold)
- [germanStandardFanfold](GC.Spread.Sheets.Print.PaperKind.md#germanstandardfanfold)
- [inviteEnvelope](GC.Spread.Sheets.Print.PaperKind.md#inviteenvelope)
- [isoB4](GC.Spread.Sheets.Print.PaperKind.md#isob4)
- [italyEnvelope](GC.Spread.Sheets.Print.PaperKind.md#italyenvelope)
- [japaneseDoublePostcard](GC.Spread.Sheets.Print.PaperKind.md#japanesedoublepostcard)
- [japaneseDoublePostcardRotated](GC.Spread.Sheets.Print.PaperKind.md#japanesedoublepostcardrotated)
- [japaneseEnvelopeChouNumber3](GC.Spread.Sheets.Print.PaperKind.md#japaneseenvelopechounumber3)
- [japaneseEnvelopeChouNumber3Rotated](GC.Spread.Sheets.Print.PaperKind.md#japaneseenvelopechounumber3rotated)
- [japaneseEnvelopeChouNumber4](GC.Spread.Sheets.Print.PaperKind.md#japaneseenvelopechounumber4)
- [japaneseEnvelopeChouNumber4Rotated](GC.Spread.Sheets.Print.PaperKind.md#japaneseenvelopechounumber4rotated)
- [japaneseEnvelopeKakuNumber2](GC.Spread.Sheets.Print.PaperKind.md#japaneseenvelopekakunumber2)
- [japaneseEnvelopeKakuNumber2Rotated](GC.Spread.Sheets.Print.PaperKind.md#japaneseenvelopekakunumber2rotated)
- [japaneseEnvelopeKakuNumber3](GC.Spread.Sheets.Print.PaperKind.md#japaneseenvelopekakunumber3)
- [japaneseEnvelopeKakuNumber3Rotated](GC.Spread.Sheets.Print.PaperKind.md#japaneseenvelopekakunumber3rotated)
- [japaneseEnvelopeYouNumber4](GC.Spread.Sheets.Print.PaperKind.md#japaneseenvelopeyounumber4)
- [japaneseEnvelopeYouNumber4Rotated](GC.Spread.Sheets.Print.PaperKind.md#japaneseenvelopeyounumber4rotated)
- [japanesePostcard](GC.Spread.Sheets.Print.PaperKind.md#japanesepostcard)
- [japanesePostcardRotated](GC.Spread.Sheets.Print.PaperKind.md#japanesepostcardrotated)
- [ledger](GC.Spread.Sheets.Print.PaperKind.md#ledger)
- [legal](GC.Spread.Sheets.Print.PaperKind.md#legal)
- [legalExtra](GC.Spread.Sheets.Print.PaperKind.md#legalextra)
- [letter](GC.Spread.Sheets.Print.PaperKind.md#letter)
- [letterExtra](GC.Spread.Sheets.Print.PaperKind.md#letterextra)
- [letterExtraTransverse](GC.Spread.Sheets.Print.PaperKind.md#letterextratransverse)
- [letterPlus](GC.Spread.Sheets.Print.PaperKind.md#letterplus)
- [letterRotated](GC.Spread.Sheets.Print.PaperKind.md#letterrotated)
- [letterSmall](GC.Spread.Sheets.Print.PaperKind.md#lettersmall)
- [letterTransverse](GC.Spread.Sheets.Print.PaperKind.md#lettertransverse)
- [monarchEnvelope](GC.Spread.Sheets.Print.PaperKind.md#monarchenvelope)
- [note](GC.Spread.Sheets.Print.PaperKind.md#note)
- [number10Envelope](GC.Spread.Sheets.Print.PaperKind.md#number10envelope)
- [number11Envelope](GC.Spread.Sheets.Print.PaperKind.md#number11envelope)
- [number12Envelope](GC.Spread.Sheets.Print.PaperKind.md#number12envelope)
- [number14Envelope](GC.Spread.Sheets.Print.PaperKind.md#number14envelope)
- [number9Envelope](GC.Spread.Sheets.Print.PaperKind.md#number9envelope)
- [personalEnvelope](GC.Spread.Sheets.Print.PaperKind.md#personalenvelope)
- [prc16K](GC.Spread.Sheets.Print.PaperKind.md#prc16k)
- [prc16KRotated](GC.Spread.Sheets.Print.PaperKind.md#prc16krotated)
- [prc32K](GC.Spread.Sheets.Print.PaperKind.md#prc32k)
- [prc32KBig](GC.Spread.Sheets.Print.PaperKind.md#prc32kbig)
- [prc32KBigRotated](GC.Spread.Sheets.Print.PaperKind.md#prc32kbigrotated)
- [prc32KRotated](GC.Spread.Sheets.Print.PaperKind.md#prc32krotated)
- [prcEnvelopeNumber1](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber1)
- [prcEnvelopeNumber10](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber10)
- [prcEnvelopeNumber10Rotated](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber10rotated)
- [prcEnvelopeNumber1Rotated](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber1rotated)
- [prcEnvelopeNumber2](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber2)
- [prcEnvelopeNumber2Rotated](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber2rotated)
- [prcEnvelopeNumber3](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber3)
- [prcEnvelopeNumber3Rotated](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber3rotated)
- [prcEnvelopeNumber4](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber4)
- [prcEnvelopeNumber4Rotated](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber4rotated)
- [prcEnvelopeNumber5](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber5)
- [prcEnvelopeNumber5Rotated](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber5rotated)
- [prcEnvelopeNumber6](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber6)
- [prcEnvelopeNumber6Rotated](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber6rotated)
- [prcEnvelopeNumber7](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber7)
- [prcEnvelopeNumber7Rotated](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber7rotated)
- [prcEnvelopeNumber8](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber8)
- [prcEnvelopeNumber8Rotated](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber8rotated)
- [prcEnvelopeNumber9](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber9)
- [prcEnvelopeNumber9Rotated](GC.Spread.Sheets.Print.PaperKind.md#prcenvelopenumber9rotated)
- [quarto](GC.Spread.Sheets.Print.PaperKind.md#quarto)
- [standard10x11](GC.Spread.Sheets.Print.PaperKind.md#standard10x11)
- [standard10x14](GC.Spread.Sheets.Print.PaperKind.md#standard10x14)
- [standard11x17](GC.Spread.Sheets.Print.PaperKind.md#standard11x17)
- [standard12x11](GC.Spread.Sheets.Print.PaperKind.md#standard12x11)
- [standard15x11](GC.Spread.Sheets.Print.PaperKind.md#standard15x11)
- [standard9x11](GC.Spread.Sheets.Print.PaperKind.md#standard9x11)
- [statement](GC.Spread.Sheets.Print.PaperKind.md#statement)
- [tabloid](GC.Spread.Sheets.Print.PaperKind.md#tabloid)
- [tabloidExtra](GC.Spread.Sheets.Print.PaperKind.md#tabloidextra)
- [usStandardFanfold](GC.Spread.Sheets.Print.PaperKind.md#usstandardfanfold)

## Enumeration members

### <a id="a2" name="a2"></a> a2

• **a2** = `66`

指定纸张尺寸为 420 mm * 594 mm。

___

### <a id="a3" name="a3"></a> a3

• **a3** = `8`

指定纸张尺寸为 297 mm * 420 mm。

___

### <a id="a3extra" name="a3extra"></a> a3Extra

• **a3Extra** = `63`

指定纸张尺寸为 322 mm * 445 mm。

___

### <a id="a3extratransverse" name="a3extratransverse"></a> a3ExtraTransverse

• **a3ExtraTransverse** = `68`

指定纸张尺寸为 322 mm * 445 mm。

___

### <a id="a3rotated" name="a3rotated"></a> a3Rotated

• **a3Rotated** = `76`

指定纸张尺寸为 420 mm * 297 mm。

___

### <a id="a3transverse" name="a3transverse"></a> a3Transverse

• **a3Transverse** = `67`

指定纸张尺寸为 297 mm * 420 mm。

___

### <a id="a4" name="a4"></a> a4

• **a4** = `9`

指定纸张尺寸为 210 mm * 297 mm。

___

### <a id="a4extra" name="a4extra"></a> a4Extra

• **a4Extra** = `53`

指定纸张尺寸为 236 mm * 322 mm。

___

### <a id="a4plus" name="a4plus"></a> a4Plus

• **a4Plus** = `60`

指定纸张尺寸为 210 mm * 330 mm。

___

### <a id="a4rotated" name="a4rotated"></a> a4Rotated

• **a4Rotated** = `77`

指定纸张尺寸为 297 mm * 210 mm。

___

### <a id="a4small" name="a4small"></a> a4Small

• **a4Small** = `10`

指定纸张尺寸为 210 mm * 297 mm。

___

### <a id="a4transverse" name="a4transverse"></a> a4Transverse

• **a4Transverse** = `55`

指定纸张尺寸为 210 mm * 297 mm。

___

### <a id="a5" name="a5"></a> a5

• **a5** = `11`

指定纸张尺寸为 148 mm * 210 mm。

___

### <a id="a5extra" name="a5extra"></a> a5Extra

• **a5Extra** = `64`

指定纸张尺寸为 174 mm * 235 mm。

___

### <a id="a5rotated" name="a5rotated"></a> a5Rotated

• **a5Rotated** = `78`

指定纸张尺寸为 210 mm * 148 mm。

___

### <a id="a5transverse" name="a5transverse"></a> a5Transverse

• **a5Transverse** = `61`

指定纸张尺寸为 148 mm * 210 mm。

___

### <a id="a6" name="a6"></a> a6

• **a6** = `70`

指定纸张尺寸为 105 mm * 148 mm。

___

### <a id="a6rotated" name="a6rotated"></a> a6Rotated

• **a6Rotated** = `83`

指定纸张尺寸为 148 mm * 105 mm。

___

### <a id="aplus" name="aplus"></a> aPlus

• **aPlus** = `57`

指定纸张尺寸为 227 mm * 356 mm。

___

### <a id="b4" name="b4"></a> b4

• **b4** = `12`

指定纸张尺寸为 250 mm * 353 mm。

___

### <a id="b4envelope" name="b4envelope"></a> b4Envelope

• **b4Envelope** = `33`

指定纸张尺寸为 250 mm * 353 mm。

___

### <a id="b4jisrotated" name="b4jisrotated"></a> b4JisRotated

• **b4JisRotated** = `79`

指定纸张尺寸为 364 mm * 257 mm。

___

### <a id="b5" name="b5"></a> b5

• **b5** = `13`

指定纸张尺寸为 176 mm * 250 mm。

___

### <a id="b5envelope" name="b5envelope"></a> b5Envelope

• **b5Envelope** = `34`

指定纸张尺寸为 176 mm * 250 mm。

___

### <a id="b5extra" name="b5extra"></a> b5Extra

• **b5Extra** = `65`

指定纸张尺寸为 201 mm * 276 mm。

___

### <a id="b5jisrotated" name="b5jisrotated"></a> b5JisRotated

• **b5JisRotated** = `80`

指定纸张尺寸为 257 mm * 182 mm。

___

### <a id="b5transverse" name="b5transverse"></a> b5Transverse

• **b5Transverse** = `62`

指定纸张尺寸为 182 mm * 257 mm。

___

### <a id="b6envelope" name="b6envelope"></a> b6Envelope

• **b6Envelope** = `35`

指定纸张尺寸为 176 mm * 125 mm。

___

### <a id="b6jis" name="b6jis"></a> b6Jis

• **b6Jis** = `88`

指定纸张尺寸为 128 mm * 182 mm。

___

### <a id="b6jisrotated" name="b6jisrotated"></a> b6JisRotated

• **b6JisRotated** = `89`

指定纸张尺寸为 182 mm * 128 mm。

___

### <a id="bplus" name="bplus"></a> bPlus

• **bPlus** = `58`

指定纸张尺寸为 305 mm * 487 mm。

___

### <a id="c3envelope" name="c3envelope"></a> c3Envelope

• **c3Envelope** = `29`

指定纸张尺寸为 324 mm * 458 mm。

___

### <a id="c4envelope" name="c4envelope"></a> c4Envelope

• **c4Envelope** = `30`

指定纸张尺寸为 229 mm * 324 mm。

___

### <a id="c5envelope" name="c5envelope"></a> c5Envelope

• **c5Envelope** = `28`

指定纸张尺寸为 162 mm * 229 mm。

___

### <a id="c65envelope" name="c65envelope"></a> c65Envelope

• **c65Envelope** = `32`

指定纸张尺寸为 114 mm * 229 mm。

___

### <a id="c6envelope" name="c6envelope"></a> c6Envelope

• **c6Envelope** = `31`

指定纸张尺寸为 114 mm * 162 mm。

___

### <a id="csheet" name="csheet"></a> cSheet

• **cSheet** = `24`

指定纸张尺寸为 17 英寸 * 22 英寸。

___

### <a id="custom" name="custom"></a> custom

• **custom** = `0`

指定纸张尺寸由用户定义。

___

### <a id="dsheet" name="dsheet"></a> dSheet

• **dSheet** = `25`

指定纸张尺寸为 22 英寸 * 34 英寸。

___

### <a id="dlenvelope" name="dlenvelope"></a> dlEnvelope

• **dlEnvelope** = `27`

指定纸张尺寸为 110 mm * 220 mm。

___

### <a id="esheet" name="esheet"></a> eSheet

• **eSheet** = `26`

指定纸张尺寸为 34 英寸 * 44 英寸。

___

### <a id="executive" name="executive"></a> executive

• **executive** = `7`

指定纸张尺寸为 7.25 英寸 * 10.5 英寸。

___

### <a id="folio" name="folio"></a> folio

• **folio** = `14`

指定纸张尺寸为 8.5 英寸 * 13 英寸。

___

### <a id="germanlegalfanfold" name="germanlegalfanfold"></a> germanLegalFanfold

• **germanLegalFanfold** = `41`

指定纸张尺寸为 8.5 英寸 * 13 英寸。

___

### <a id="germanstandardfanfold" name="germanstandardfanfold"></a> germanStandardFanfold

• **germanStandardFanfold** = `40`

指定纸张尺寸为 8.5 英寸 * 12 英寸。

___

### <a id="inviteenvelope" name="inviteenvelope"></a> inviteEnvelope

• **inviteEnvelope** = `47`

指定纸张尺寸为 220 mm * 220 mm。

___

### <a id="isob4" name="isob4"></a> isoB4

• **isoB4** = `42`

指定纸张尺寸为 250 mm * 353 mm。

___

### <a id="italyenvelope" name="italyenvelope"></a> italyEnvelope

• **italyEnvelope** = `36`

指定纸张尺寸为 110 mm * 230 mm。

___

### <a id="japanesedoublepostcard" name="japanesedoublepostcard"></a> japaneseDoublePostcard

• **japaneseDoublePostcard** = `69`

指定纸张尺寸为 200 mm * 148 mm。

___

### <a id="japanesedoublepostcardrotated" name="japanesedoublepostcardrotated"></a> japaneseDoublePostcardRotated

• **japaneseDoublePostcardRotated** = `82`

指定纸张尺寸为 148 mm * 200 mm。

___

### <a id="japaneseenvelopechounumber3" name="japaneseenvelopechounumber3"></a> japaneseEnvelopeChouNumber3

• **japaneseEnvelopeChouNumber3** = `73`

指定纸张尺寸为日本 Chou #3 信封，120 mm * 235 mm。

___

### <a id="japaneseenvelopechounumber3rotated" name="japaneseenvelopechounumber3rotated"></a> japaneseEnvelopeChouNumber3Rotated

• **japaneseEnvelopeChouNumber3Rotated** = `86`

指定纸张尺寸为日本旋转 Chou #3 信封，235 mm * 120 mm。

___

### <a id="japaneseenvelopechounumber4" name="japaneseenvelopechounumber4"></a> japaneseEnvelopeChouNumber4

• **japaneseEnvelopeChouNumber4** = `74`

指定纸张尺寸为日本 Chou #4 信封，90 mm * 205 mm。

___

### <a id="japaneseenvelopechounumber4rotated" name="japaneseenvelopechounumber4rotated"></a> japaneseEnvelopeChouNumber4Rotated

• **japaneseEnvelopeChouNumber4Rotated** = `87`

指定纸张尺寸为日本旋转 Chou #4 信封，205 mm * 90 mm。

___

### <a id="japaneseenvelopekakunumber2" name="japaneseenvelopekakunumber2"></a> japaneseEnvelopeKakuNumber2

• **japaneseEnvelopeKakuNumber2** = `71`

指定纸张尺寸为日本 Kaku #2 信封，240 mm * 332 mm。

___

### <a id="japaneseenvelopekakunumber2rotated" name="japaneseenvelopekakunumber2rotated"></a> japaneseEnvelopeKakuNumber2Rotated

• **japaneseEnvelopeKakuNumber2Rotated** = `84`

指定纸张尺寸为日本旋转 Kaku #2 信封，332 mm * 240 mm。

___

### <a id="japaneseenvelopekakunumber3" name="japaneseenvelopekakunumber3"></a> japaneseEnvelopeKakuNumber3

• **japaneseEnvelopeKakuNumber3** = `72`

指定纸张尺寸为日本 Kaku #3 信封，216 mm * 277 mm。

___

### <a id="japaneseenvelopekakunumber3rotated" name="japaneseenvelopekakunumber3rotated"></a> japaneseEnvelopeKakuNumber3Rotated

• **japaneseEnvelopeKakuNumber3Rotated** = `85`

指定纸张尺寸为日本旋转 Kaku #3 信封，277 mm * 216 mm。

___

### <a id="japaneseenvelopeyounumber4" name="japaneseenvelopeyounumber4"></a> japaneseEnvelopeYouNumber4

• **japaneseEnvelopeYouNumber4** = `91`

指定纸张尺寸为日本 You #4 信封，235 mm * 105 mm。

___

### <a id="japaneseenvelopeyounumber4rotated" name="japaneseenvelopeyounumber4rotated"></a> japaneseEnvelopeYouNumber4Rotated

• **japaneseEnvelopeYouNumber4Rotated** = `92`

指定纸张尺寸为日本旋转 You #4 信封，105 mm * 235 mm。

___

### <a id="japanesepostcard" name="japanesepostcard"></a> japanesePostcard

• **japanesePostcard** = `43`

指定纸张尺寸为 100 mm * 148 mm。

___

### <a id="japanesepostcardrotated" name="japanesepostcardrotated"></a> japanesePostcardRotated

• **japanesePostcardRotated** = `81`

指定纸张尺寸为 148 mm * 100 mm。

___

### <a id="ledger" name="ledger"></a> ledger

• **ledger** = `4`

指定纸张尺寸为 17 英寸 * 11 英寸。

___

### <a id="legal" name="legal"></a> legal

• **legal** = `5`

指定纸张尺寸为 8.5 英寸 * 14 英寸。

___

### <a id="legalextra" name="legalextra"></a> legalExtra

• **legalExtra** = `51`

指定纸张尺寸为 legal 加长纸张（9.275 英寸 * 15 英寸）。
此值特定于 PostScript 驱动程序，仅由 Linotronic 打印机使用以节省纸张。

___

### <a id="letter" name="letter"></a> letter

• **letter** = `1`

指定纸张尺寸为 8.5 英寸 * 11 英寸。

___

### <a id="letterextra" name="letterextra"></a> letterExtra

• **letterExtra** = `50`

指定纸张尺寸为 letter 加长纸张（9.275 英寸 * 12 英寸）。
此值特定于 PostScript 驱动程序，仅由 Linotronic 打印机使用以节省纸张。

___

### <a id="letterextratransverse" name="letterextratransverse"></a> letterExtraTransverse

• **letterExtraTransverse** = `56`

指定纸张尺寸为 9.275 英寸 * 12 英寸。

___

### <a id="letterplus" name="letterplus"></a> letterPlus

• **letterPlus** = `59`

指定纸张尺寸为 8.5 英寸 * 12.69 英寸。

___

### <a id="letterrotated" name="letterrotated"></a> letterRotated

• **letterRotated** = `75`

指定纸张尺寸为 11 英寸 * 8.5 英寸。

___

### <a id="lettersmall" name="lettersmall"></a> letterSmall

• **letterSmall** = `2`

指定纸张尺寸为 8.5 英寸 * 11 英寸。

___

### <a id="lettertransverse" name="lettertransverse"></a> letterTransverse

• **letterTransverse** = `54`

指定纸张尺寸为 8.275 英寸 * 11 英寸。

___

### <a id="monarchenvelope" name="monarchenvelope"></a> monarchEnvelope

• **monarchEnvelope** = `37`

指定纸张尺寸为 3.875 英寸 * 7.5 英寸。

___

### <a id="note" name="note"></a> note

• **note** = `18`

指定纸张尺寸为 8.5 英寸 * 11 英寸。

___

### <a id="number10envelope" name="number10envelope"></a> number10Envelope

• **number10Envelope** = `20`

指定纸张尺寸为 4.125 英寸 * 9.5 英寸。

___

### <a id="number11envelope" name="number11envelope"></a> number11Envelope

• **number11Envelope** = `21`

指定纸张尺寸为 4.5 英寸 * 10.375 英寸。

___

### <a id="number12envelope" name="number12envelope"></a> number12Envelope

• **number12Envelope** = `22`

指定纸张尺寸为 4.75 英寸 * 11 英寸。

___

### <a id="number14envelope" name="number14envelope"></a> number14Envelope

• **number14Envelope** = `23`

指定纸张尺寸为 5 英寸 * 11.5 英寸。

___

### <a id="number9envelope" name="number9envelope"></a> number9Envelope

• **number9Envelope** = `19`

指定纸张尺寸为 3.875 英寸 * 8.875 英寸。

___

### <a id="personalenvelope" name="personalenvelope"></a> personalEnvelope

• **personalEnvelope** = `38`

指定纸张尺寸为 3.625 英寸 * 6.5 英寸。

___

### <a id="prc16k" name="prc16k"></a> prc16K

• **prc16K** = `93`

指定纸张尺寸为 146 mm * 215 mm。

___

### <a id="prc16krotated" name="prc16krotated"></a> prc16KRotated

• **prc16KRotated** = `106`

指定纸张尺寸为 146 mm * 215 mm。

___

### <a id="prc32k" name="prc32k"></a> prc32K

• **prc32K** = `94`

指定纸张尺寸为 97 mm * 151 mm。

___

### <a id="prc32kbig" name="prc32kbig"></a> prc32KBig

• **prc32KBig** = `95`

指定纸张尺寸为 97 mm * 151 mm。

___

### <a id="prc32kbigrotated" name="prc32kbigrotated"></a> prc32KBigRotated

• **prc32KBigRotated** = `108`

指定纸张尺寸为 97 mm * 151 mm。

___

### <a id="prc32krotated" name="prc32krotated"></a> prc32KRotated

• **prc32KRotated** = `107`

指定纸张尺寸为 97 mm * 151 mm。

___

### <a id="prcenvelopenumber1" name="prcenvelopenumber1"></a> prcEnvelopeNumber1

• **prcEnvelopeNumber1** = `96`

指定纸张尺寸为 102 mm * 165 mm。

___

### <a id="prcenvelopenumber10" name="prcenvelopenumber10"></a> prcEnvelopeNumber10

• **prcEnvelopeNumber10** = `105`

指定纸张尺寸为 324 mm * 458 mm。

___

### <a id="prcenvelopenumber10rotated" name="prcenvelopenumber10rotated"></a> prcEnvelopeNumber10Rotated

• **prcEnvelopeNumber10Rotated** = `118`

指定纸张尺寸为 458 mm * 324 mm。

___

### <a id="prcenvelopenumber1rotated" name="prcenvelopenumber1rotated"></a> prcEnvelopeNumber1Rotated

• **prcEnvelopeNumber1Rotated** = `109`

指定纸张尺寸为 165 mm * 102 mm。

___

### <a id="prcenvelopenumber2" name="prcenvelopenumber2"></a> prcEnvelopeNumber2

• **prcEnvelopeNumber2** = `97`

指定纸张尺寸为 102 mm * 176 mm。

___

### <a id="prcenvelopenumber2rotated" name="prcenvelopenumber2rotated"></a> prcEnvelopeNumber2Rotated

• **prcEnvelopeNumber2Rotated** = `110`

指定纸张尺寸为 176 mm * 102 mm。

___

### <a id="prcenvelopenumber3" name="prcenvelopenumber3"></a> prcEnvelopeNumber3

• **prcEnvelopeNumber3** = `98`

指定纸张尺寸为 125 mm * 176 mm。

___

### <a id="prcenvelopenumber3rotated" name="prcenvelopenumber3rotated"></a> prcEnvelopeNumber3Rotated

• **prcEnvelopeNumber3Rotated** = `111`

指定纸张尺寸为 176 mm * 125 mm。

___

### <a id="prcenvelopenumber4" name="prcenvelopenumber4"></a> prcEnvelopeNumber4

• **prcEnvelopeNumber4** = `99`

指定纸张尺寸为 110 mm * 208 mm。

___

### <a id="prcenvelopenumber4rotated" name="prcenvelopenumber4rotated"></a> prcEnvelopeNumber4Rotated

• **prcEnvelopeNumber4Rotated** = `112`

指定纸张尺寸为 208 mm * 110 mm。

___

### <a id="prcenvelopenumber5" name="prcenvelopenumber5"></a> prcEnvelopeNumber5

• **prcEnvelopeNumber5** = `100`

指定纸张尺寸为 110 mm * 220 mm。

___

### <a id="prcenvelopenumber5rotated" name="prcenvelopenumber5rotated"></a> prcEnvelopeNumber5Rotated

• **prcEnvelopeNumber5Rotated** = `113`

指定纸张尺寸为 220 mm * 110 mm。

___

### <a id="prcenvelopenumber6" name="prcenvelopenumber6"></a> prcEnvelopeNumber6

• **prcEnvelopeNumber6** = `101`

指定纸张尺寸为 120 mm * 230 mm。

___

### <a id="prcenvelopenumber6rotated" name="prcenvelopenumber6rotated"></a> prcEnvelopeNumber6Rotated

• **prcEnvelopeNumber6Rotated** = `114`

指定纸张尺寸为 230 mm * 120 mm。

___

### <a id="prcenvelopenumber7" name="prcenvelopenumber7"></a> prcEnvelopeNumber7

• **prcEnvelopeNumber7** = `102`

指定纸张尺寸为 160 mm * 230 mm。

___

### <a id="prcenvelopenumber7rotated" name="prcenvelopenumber7rotated"></a> prcEnvelopeNumber7Rotated

• **prcEnvelopeNumber7Rotated** = `115`

指定纸张尺寸为 230 mm * 160 mm。

___

### <a id="prcenvelopenumber8" name="prcenvelopenumber8"></a> prcEnvelopeNumber8

• **prcEnvelopeNumber8** = `103`

指定纸张尺寸为 120 mm * 309 mm。

___

### <a id="prcenvelopenumber8rotated" name="prcenvelopenumber8rotated"></a> prcEnvelopeNumber8Rotated

• **prcEnvelopeNumber8Rotated** = `116`

指定纸张尺寸为 309 mm * 120 mm。

___

### <a id="prcenvelopenumber9" name="prcenvelopenumber9"></a> prcEnvelopeNumber9

• **prcEnvelopeNumber9** = `104`

指定纸张尺寸为 229 mm * 324 mm。

___

### <a id="prcenvelopenumber9rotated" name="prcenvelopenumber9rotated"></a> prcEnvelopeNumber9Rotated

• **prcEnvelopeNumber9Rotated** = `117`

指定纸张尺寸为 324 mm * 229 mm。

___

### <a id="quarto" name="quarto"></a> quarto

• **quarto** = `15`

指定纸张尺寸为 215 mm * 275 mm。

___

### <a id="standard10x11" name="standard10x11"></a> standard10x11

• **standard10x11** = `45`

指定纸张尺寸为 10 英寸 * 11 英寸。

___

### <a id="standard10x14" name="standard10x14"></a> standard10x14

• **standard10x14** = `16`

指定纸张尺寸为 10 英寸 * 14 英寸。

___

### <a id="standard11x17" name="standard11x17"></a> standard11x17

• **standard11x17** = `17`

指定纸张尺寸为 11 英寸 * 17 英寸。

___

### <a id="standard12x11" name="standard12x11"></a> standard12x11

• **standard12x11** = `90`

指定纸张尺寸为 12 英寸 * 11 英寸。

___

### <a id="standard15x11" name="standard15x11"></a> standard15x11

• **standard15x11** = `46`

指定纸张尺寸为 15 英寸 * 11 英寸。

___

### <a id="standard9x11" name="standard9x11"></a> standard9x11

• **standard9x11** = `44`

指定纸张尺寸为 9 英寸 * 11 英寸。

___

### <a id="statement" name="statement"></a> statement

• **statement** = `6`

指定纸张尺寸为 5.5 英寸 * 8.5 英寸。

___

### <a id="tabloid" name="tabloid"></a> tabloid

• **tabloid** = `3`

指定纸张尺寸为 11 英寸 * 17 英寸。

___

### <a id="tabloidextra" name="tabloidextra"></a> tabloidExtra

• **tabloidExtra** = `52`

指定纸张尺寸为 11.69 英寸 * 18 英寸。

___

### <a id="usstandardfanfold" name="usstandardfanfold"></a> usStandardFanfold

• **usStandardFanfold** = `39`

指定纸张尺寸为 14.875 英寸 * 11 英寸。

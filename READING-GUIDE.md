# 閱讀與定位

每個page.id是固定物理面識別，未必等同原刻葉碼。page.source.uri連官方canvas，image_uri連官方原圖；source_face_mapping說明安全半面與母圖關係，非逐字座標。p129–137不在本包。

面內直欄由右至左、欄內自上而下。正文、圖題、圖字、小註及版心各自以role/layer區分。小註的anchor、attach_after_unit、resume_at_unit等保存實際掛接；分列文字以換行保留。部分舊欄被註分開，勿把欄末與下一欄強接。p101小註依原像素回圖裁定，原讀序未解已解除。

原刻「、」「○」直接保留；TXT單元之間新增的換行只是檔案分隔，不是原刻句讀。沒有新增閱讀標點或全域簡繁、異體統一。

□表示已定位的單字未解；⟦g…⟧為穩定字形ID，可能代表多個原字，實際extent見UNCERTAINTIES。不可按標記字串長度估算底本字數。保留當前字也可能有uncertainty，例如p019道及p127會。

字元位置為從0起算Unicode碼點，end不含尾端，非UTF-16索引。UNCERTAINTIES的start/end對應指定unit.text；TXT範圍另見text.sidecar。TEI內u號對應tei.sidecar，不是原刻欄號。

本版ANCHORS另列正文中途的小註、續文、跨欄接註及混合字級；TXT各單元換行是交換分隔，不能直接當原刻句讀或連續閱讀順序。未定孤立墨痕在WHOLE-PAGE-LAYERS中另記，不自動化成缺字。

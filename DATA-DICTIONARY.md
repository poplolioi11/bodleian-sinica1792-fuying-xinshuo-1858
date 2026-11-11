# 資料欄位

book.json根欄位包含id/title/version/source/publication_status/pages/units。pages依固定來源序，units依頁序及保存的文字層單位序。

page.source含官方uri/image_uri、固定來源SHA-256與實際尺寸。這些尺寸可能是整幅或安全半面，請看source_face_mapping。unit.bbox=null表示沒有可靠單位框，不代表來源空白。

unit.text保留原文字串；id穩定、order供交換、page_id指原面。layer及role區分正文、段題、目錄、圖字、圖題、小註、版心及題記。required_layers/layer_states是本版實際處理宣告；p023另存已實讀但沒有圖內標字的source_layer_absence。

uncertainties包含候選、理由、狀態、碼點範圍及已知extent；gaps區分reading-unresolved/image-insufficient，與unprocessed不同。本版無unprocessed。extent不是候選數，也不是準確率。

book.json可由共用pages-units adapter無損匯入。TXT與TEI的sidecar保留單位、頁、順序、邊界及雜湊；JSON仍是完整結構主本。

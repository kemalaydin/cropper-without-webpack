## Cropper Genel Ayarları

> !! Henüz Paket Haline Getirilmemiştir.

### `cropper_aspect_x`
Cropper için aspect değerlerinden x bağımlılığını düzenler. Kullanabilmek için sayfa içerisinde id değeri `cropper_aspect_x` olan bir gizli input kullanabilirsiniz. Vereceğiniz value aspect_x değerini belirleyecektir.

Ex.
`<input type="hidden" id="cropper_aspect_x" value="100" />`

### `cropper_aspect_y`
Cropper için aspect değerlerinden y bağımlılığını düzenler. Kullanabilmek için sayfa içerisinde id değeri `cropper_aspect_y` olan bir gizli input kullanabilirsiniz. Vereceğiniz value aspect_x değerini belirleyecektir.

Ex.
`<input type="hidden" id="cropper_aspect_y" value="100" />`

### `placeholder_text`
Crop işlemi yapılan resim için açıklama inputuna ait placeholder yazısı.
Ex.
`<input type="hidden" id="cropper_aspect_y" value="100" />`


## Cropper Stil Tanımlamaları
Cropper içerisinde kullanılan inputların ve resimlerin classları mevcuttur. Bu classları bypass ederek kendi sisteminize uygun hala getirebilirsiniz.

### `.cropper_image_select`
Resim seçiçi inputun classıdır. File tipinde bir inputtur.

### `.imageSelectedMultiple`
Yüklenen resimlerin tamamını barındıran container class.

### `.singleImageMultiple`
Yüklenen her bir resmin container class'ı

### `.ReactCrop__image`
Yüklenen her bir resmin class'ı. ( Direkt olarak img tagına ait class )

### `.cropper_image_title`
Yüklenen her resmin sahip olduğu Başlık inputu class'ı. Text tipinde bir inputtur.

### `.crop_check_button`
Cropper'a yüklenen resimlerin croplama işlemini tamamlatan span sınıfı.

### `.crop_back_button`
Cropperlanan resmi tekrar croplanabilir yapan span sınıfı.


## Cropper Çıktıları
Her yüklenen resim için cropper aynı isimde inputlar oluşturur. Bu inputları sunucu tarafınızda array olarak karşılayabilirsiniz.

### `name="cropper_image[]"`
Hidden tipinde bir inputtur. Kırpılan resmin base64 kodlarını barındırır. Birden fazla resim olması durumunda array formatında veri döndürür.  -- Hidden nesnedir, sayfada kullanıcıya gösterilmez. --

### `name="cropper_input_1[]"`
Text tipinde bir inputtur. Eklenen resim için herhangi bir bilgi barındırır. Birden fazla resim olması durumunda array formatında veri döndürür. ( Bu özellik 1...6 arasındadır. - max: cropper_input_6)

### `name="cropper_input_1_placeholder[]"`
Text tipinde bir inputtur. Eklenen resim için herhangi bir bilgi barındıran inputun placeholder bilgisini ayarlar. ( Bu özellik 1...6 arasındadır. - max: cropper_input_6_placeholde)


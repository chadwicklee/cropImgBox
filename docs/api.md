
# CropImgBox API
---

## ѡ��

ѡ�� | ���� | Ĭ��ֵ | ����
--- | ---- | ------- | -----------
thumbBox | string | `''` | ѡȡ�����
spinner      | string | `''` | ͼ��չʾ����
expandRatio | integer | 1.1 | �Ŵ���
narrowRatio      | integer | 0.9 | ��С����

## ����

```javascript
// init a cropimgbox
var options =
{
    thumbBox: '.cropimgbox-thumbBox',
    spinner: '.cropimgbox-spinner',
    imgSrc: ''
}
var cropper = $('.cropimgbox-imageBox').cropimgbox(options);

// Get the imgs
cropper.getDataURL(function (arrs) {
})

// expand image
cropper.zoomIn();

// narrow image
cropper.zoomOut();

//converted base64 to Blod for upload files
cropper.getBlob(i);
```

����        | ����      | ����
------     | -------- | -----------
cropimgbox      | options : object | ��ʼ�� cropimgbox
getDataURL    | callback  | ��ȡ��ȡ�任���ͼ��base64����
zoomIn  |  | �Ŵ�
zoomOut  | | ��С
getBlob  | i:int | ��base64ת��ΪBlob,iΪ������±�

mcu GW5_CropWOI()
default is 1:center
    uint8_t data[] = {0x04, 0x00, 0x02};
    uint8_t dataWOI[WOI_TABLE_MAX][32] ={ //0 Down, 1 Center , 2 Top
        {0x02, 0x01, 0x00, 0x00, 0x00, 0x00, 0x70, 0x44, 0x00, 0x00, 0x57, 0x44, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0xd1, 0x5e, 0x02, 0x43, 0x00, 0x00, 0x80, 0x3f, 0xb4, 0x97, 0xd0, 0x3e},               
        # {0x02, 0x01, 0x00, 0x00, ==0x00, 0x00, 0x70, 0x44==, 0x00, 0x80, 0x22, 0x44, ==0x00, 0x00, 0x00, 0x00,== 0x00, 0x00, 0x00, 0x00, ==0x5f, 0x42, 0x33, 0x42,== 0x00, 0x00, 0x80, 0x3f, ==0xb4, 0x97, 0xd0, 0x3e==},
        {0x02, 0x01, 0x00, 0x00, 0x00, 0x00, 0x70, 0x44, 0x00, 0x00, 0xdc, 0x43, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x85, 0xf6, 0x22, 0xc2, 0x00, 0x00, 0x80, 0x3f, 0xb4, 0x97, 0xd0, 0x3e},
api_cmd.exe -I 0x4D 0 040002
api_cmd.exe -I 0x4E 0 02010000\f960\\f221\\f0\\f0\\f-129.962962962963\\f1\\f0.407407407407407\
api_cmd.exe -I 0x4D 0 \s4\02
api_cmd.exe -I 0x4E 0
02010000\f960\\f540\\f0\\f0\\f0\\f1\\f0.407407407407407\

typedef struct {
    float ==centerX==;                  /*!< X-centering of output warp. In terms of pixels. Suggest setting to the center X-coordinate of original output resolution. */
    float centerY;                  /*!< Y-centering of output warp. In terms of pixels. Suggest setting to the center Y-coordinate of original output resolution. */
    float ==rotateZ==;                  /*!< Output warp rotation of the XY-plane (i.e. 2D) around \ref centerX and \ref centerY. In terms of degrees. Set to 0 for no rotation. */
    float shiftX;                   /*!< Output warp shifting (panning) along X-dimension. In terms of pixels. Set to 0 for no shifting */
    float ==shiftY==;                   /*!< Output warp shifting (panning) along Y-dimension. In terms of pixels. Set to 0 for no shifting */
    float scaleX;                   /*!< Output warp scaling (zooming-in) along X-dimension. Set to 1 for no scaling. Must not be greater than 1. */
    float ==scaleY==;                   /*!< Output warp scaling (zooming-in) along Y-dimension. Set to 1 for no scaling. Must not be greater than 1. */
} OutWarpAdjParams_s;


WOI excel 

outspace_warpmap_adjustment_howto.xlsx
down
![[Pasted image 20241218162112.png | 100 ]]
center
![[Pasted image 20241218171039.png |100]]
top
![[Pasted image 20241218171133.png | 100]]
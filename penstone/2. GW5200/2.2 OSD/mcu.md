API_CODE_CONFIG_OSD_CHANNEL             (0x27U)  //draw icon
API_CODE_VG_DRAW_PRIMITIVES             (0x30U) //draw line in 0x17000 vg_on

#pragma pack(1)  0x27
typedef struct {
    uint8_t channel;         /*!< OSD channel index, 0 ... (\ref GW5_OSD_NUM_CHANNELS - 1) */
    uint8_t enable;
    uint8_t alpha;
    uint8_t pad[1];          /*!< Padding (set to 0x00) */
    uint16_t offsetX;
    uint16_t offsetY;
    uint8_t imageSlotId;     /*!< OSD image slot ID. The size of an image slot is specified in syscfg JSON osdConfig.imageSlotSize. */
    uint8_t clutSlotId;      /*!< OSD CLUT slot ID. The maximum number of CLUT slots is specified in syscfg JSON osdConfig.numClutSlots. */
} ConfigOsdChannel_s;
#pragma pack(0)

<font color="red">channel</font>
1 channel only can show 1 icon at same time, if show 2 icon, need put difference channel

ALDrawOSD_LoadImageSlot 0x25 image ID -> slot ID  (imageID, imageID-1)  1->0, 2->1,...,9->8
ALDrawOSD_LoadClutSlot 0x26 Clut ID-> Slot ID
ALDrawOSD_ConfigOsdChannel 0x27 
12->11 slot *(OSD_ID_HIGHLIGHT_1)*
api_cmd.exe -I 0x25 0 80000c000d
api_cmd.exe -I 0x26 0 80000c000d
api_cmd.exe -I 0x27 0 *0201ff00330033000d0d*
typedef enum OSD_ID {
    OSD_ID_RESERVER ,//OSD ID is from 1 ~
    OSD_ID_BLACK_LINE_1 ,
    OSD_ID_BLACK_LINE_2 , 
    OSD_ID_BRIGHT_1 ,
    OSD_ID_BRIGHT_2 , 
    OSD_ID_BRIGHT_3 ,
    OSD_ID_BRIGHT_4 ,
    OSD_ID_BRIGHT_5 ,
    OSD_ID_C_PILLAR ,
    OSD_ID_WOI_1 ,
    OSD_ID_WOI_2 ,
    OSD_ID_WOI_3 ,
    OSD_ID_HIGHLIGHT_1 ,          
    OSD_ID_TOTAL ,  
} OSD_ID;


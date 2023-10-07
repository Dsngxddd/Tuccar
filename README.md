> Eklentinin artık geliştirilmemektedir.

> 1.13 ve üzeri bir sürümde kullanıyorsanız .jar dosyasını winrar ile açıp 1.16 config dosyasını mevcut config dosyasıyla değiştirin!

# Tuccar

Tüccar bir oyun içi oyuncu marketi eklentisidir. 

## Nasıl çalışıyor?

Görevli bir NPC ile çalışan bu eklenti oyuncuların kendi eşyalarını diğer oyunculara satması şeklinde çalışır. İtemleri otomatik olarak kategorize edip bulunması kolay olayacak şekilde listeleyen bu oyuncu market eklentisi aynı kategoride olan eşyaları fiyata göre akıllı listeleme özelliğine de sahip. Oyuncuların online olmaması durumunu göz önünde bulundurarak satılan eşyaları veya alınan eşyaları kendi envanterinde saklayarak oyunculara istediği zaman marketten geri çekmesine olanak sağlar.

## Config ve Dil dosyası
<details>
  <summary>config.yml</summary>
    Settings:
    # SHIFT + SOL tık ile alınacak adet sayısıdır.
    customBuyAmount: 32
    # Minimum listelenecek satış fiyatı
    minimumPrice: 1
    # Tüccar komut ile açılabilsin mi? /tüccar
    openTuccarViaCmd: false
    # Kategori seçme menüsünün büyüklüğünü belirler
    categorySize: 36
    # Orta tuş ile fiyat güncelleme ayarı.
    middleClickRePrice: true
    # Tüccarın kullanılabileceği dünyaları belirler.
    world:
        # Dünya beyaz listesi aktif edilsin mi?
        worldWhitelist: true
        # Dünya beyaz listesi aktifse hangi dünyalarda çalışsın.
        allowedWorlds:
        - world
    Tax:
    # Alınan vergi bir hesaba yatırılsın mı?
    depositAccount: false
    # Vergi bir hesaba yatırılıyorsa hangi hesap?
    account: Geyik
    # Vergi oranı % kaçtır? 0 yazarak devre dışı bırakabilirsiniz.
    taxRate: 0
    # Ana tüccar bloğudur. Blok ile başlayan kısım kategoridir.
    # Özel kategori oluşturmak için onun gibi yeni bir isim yazabilirsiniz.
    # Aşağıda belirli bilgiler mevcuttur:
    # KATEGORİLER #
    # displayName: Kategorinin görünen adıdır. (Zorunlu)
    # displayLore: Kategorinin görünen açıklamasıdır. (Zorunlu)
    # slot: Kategorinin olması gereken slotudur. (Zorunlu)
    # material: Kategorinin materyalidir. (Zorunlu)
    #
    # ÜRÜNLER #
    # displayName: Eşyanın tüccar guisi üzerinde gözükeceği isim (silinebilir)
    # displayLore: Eşyanın tüccar guisi üzerinde gözükecek açıklaması (silinebilir)
    # itemName: Eşyanın listelenebilmesi için gerekli olan ismidir. Örneğin: itemName: "&6Uçuş Kağıdı" (silinebilir)
    # damage: Eşyanın hasarıdır. 1.8 ve 1.12 arasında geçerlidir. (silinebilir.)
    # material: Eşyanın materyalidir. (Zorunlu)
    # enchantment: Eşyanın tüccara konması için gerekli enchantlardır. Örnek: (silinebilir)
    # enchantment:
    # - "DAMAGE_ALL:5"
    Tuccar:
    Blok:
        slot: 12
        displayName: '&6Bloklar'
        material: GRASS
        displayLore:
        - ''
        - ' &8▪ &7Bu kategoride, ihtiyacın'
        - ' &7olan &eblokları &7inceleyebilir'
        - ' &7ve satın alabilirsin.'
        - ''
        - ' &8▸ &aTıkla ve alışverişe başla!'
        items:
        1: #Birbirinden farklı sayısal değerler girmelisiniz!
            material: ICE
            displayName: '&eBuz'
        2:
            material: PACKED_ICE
            displayName: '&ePaketlenmiş Buz'
        3:
            material: MOSSY_COBBLESTONE
            displayName: '&eYosunlu Taş'
        4:
            material: BRICK
            displayName: '&eTuğla'
        5:
            material: BOOKSHELF
            displayName: '&eKitaplık'
        6:
            material: WOOD
            damage: 0
            displayName: '&eMeşe Tahtası'
        7:
            material: WOOD
            damage: 1
            displayName: '&eLadin Tahtası'
        8:
            material: WOOD
            damage: 2
            displayName: '&eHuş Tahtası'
        9:
            material: WOOD
            damage: 3
            displayName: '&eOrman Tahtası'
        10:
            material: WOOD
            damage: 4
            displayName: '&eAkasya Tahtası'
        11:
            material: WOOD
            damage: 5
            displayName: '&eKoyu Meşe Tahtası'
        12:
            material: LOG
            damage: 0
            displayName: '&eMeşe OdunU'
        13:
            material: LOG
            damage: 1
            displayName: '&eLadin Odunu'
        14:
            material: LOG
            damage: 2
            displayName: '&eHuş Odunu'
        15:
            material: LOG
            damage: 3
            displayName: '&eOrman Odunu'
        16:
            material: LOG_2
            damage: 0
            displayName: '&eAkasya Odunu'
        17:
            material: LOG_2
            damage: 1
            displayName: '&eKoyu Meşe Odunu'
        18:
            material: SPONGE
            displayName: '&eSünger'
        19:
            material: PRISMARINE
            damage: 0
            displayName: '&ePrizmarin'
        20:
            material: PRISMARINE
            damage: 1
            displayName: '&ePrizmarin Tuğlası'
        21:
            material: PRISMARINE
            damage: 2
            displayName: '&eKoyu Prizmarin'
        22:
            material: COAL_BLOCK
            displayName: '&eKömür Bloğu'
        23:
            material: OBSIDIAN
            displayName: '&eObsidyen'
        23:
            material: PUMPKIN
            displayName: '&eBalkabagi'
        24:
            material: LAPIS_BLOCK
            displayName: '&eLapis Blok'
        25:
            material: SEA_LANTERN
            displayName: '&eDeniz Feneri'
        26:
            material: GLOWSTONE
            displayName: '&eIşıktaşı'
        27:
            material: SOUL_SAND
            displayName: '&eRuh Kumu'
        28:
            material: SNOW_BLOCK
            displayName: '&eKar'
        29:
            material: QUARTZ_BLOCK
            damage: 0
            displayName: '&eKuvars Bloğu'
        29:
            material: QUARTZ_BLOCK
            damage: 1
            displayName: '&eKeskin Kuvars Bloğu'
        30:
            material: QUARTZ_BLOCK
            damage: 2
            displayName: '&eKuvars Sütun Bloğu'
        31:
            material: NETHER_BRICK
            displayName: '&eNether Tuğlası'
        32:
            material: NETHERRACK
            displayName: '&eNetherrack'
        33:
            material: SMOOTH_BRICK
            displayName: '&eTaş Tuğla'
        34:
            material: MYCEL
            displayName: '&eMiselyum'
        35:
            material: DIRT
            displayName: '&eToprak'
        36:
            material: COBBLESTONE
            displayName: '&eKırıktaş'
        37:
            material: SAND
            displayName: '&eKum'
        38:
            material: SANDSTONE
            displayName: '&eKumtaşı'
        39:
            material: ENDER_STONE
            displayName: '&eEnd Taşı'
        40:
            material: CLAY
            displayName: '&eKil'
        41:
            material: HARD_CLAY
            displayName: '&eSertleştirilmiş Kil'
        42:
            material: STAINED_CLAY
            damage: 0
            displayName: '&eBeyaz Kil'
        43:
            material: STAINED_CLAY
            damage: 1
            displayName: '&eTuruncu Kil'
        44:
            material: STAINED_CLAY
            damage: 2
            displayName: '&eEflatun Kil'
        45:
            material: STAINED_CLAY
            damage: 3
            displayName: '&eAçık Mavi Kil'
        46:
            material: STAINED_CLAY
            damage: 4
            displayName: '&eSarı Kil'
        47:
            material: STAINED_CLAY
            damage: 5
            displayName: '&eAçık Yeşil Kil'
        48:
            material: STAINED_CLAY
            damage: 6
            displayName: '&ePembe Kil'
        49:
            material: STAINED_CLAY
            damage: 7
            displayName: '&eGri Kil'
        50:
            material: STAINED_CLAY
            damage: 8
            displayName: '&eAçık Gri Kil'
        51:
            material: STAINED_CLAY
            damage: 9
            displayName: '&eCamgöbeği Kil'
        52:
            material: STAINED_CLAY
            damage: 10
            displayName: '&eMor Kil'
        53:
            material: STAINED_CLAY
            damage: 11
            displayName: '&eMavi Kil'
        54:
            material: STAINED_CLAY
            damage: 12
            displayName: '&eKahverengi Kil'
        55:
            material: STAINED_CLAY
            damage: 13
            displayName: '&eYeşil Kil'
        56:
            material: STAINED_CLAY
            damage: 14
            displayName: '&eKırmızı Kil'
        57:
            material: STAINED_CLAY
            damage: 15
            displayName: '&eSiyah Kil'
        58:
            material: WOOL
            damage: 0
            displayName: '&eBeyaz Yün'
        59:
            material: WOOL
            damage: 1
            displayName: '&eTuruncu Yün'
        60:
            material: WOOL
            damage: 2
            displayName: '&eEflatun Yün'
        61:
            material: WOOL
            damage: 3
            displayName: '&eAçık Mavi Yün'
        62:
            material: WOOL
            damage: 4
            displayName: '&eSarı Yün'
        63:
            material: WOOL
            damage: 5
            displayName: '&eAçık Yeşil Yün'
        64:
            material: WOOL
            damage: 6
            displayName: '&ePembe Yün'
        65:
            material: WOOL
            damage: 7
            displayName: '&eGri Yün'
        66:
            material: WOOL
            damage: 8
            displayName: '&eAçık Gri Yün'
        67:
            material: WOOL
            damage: 9
            displayName: '&eCamgöbeği Yün'
        68:
            material: WOOL
            damage: 10
            displayName: '&eMor Yün'
        69:
            material: WOOL
            damage: 11
            displayName: '&eMavi Yün'
        70:
            material: WOOL
            damage: 12
            displayName: '&eKahverengi Yün'
        71:
            material: WOOL
            damage: 13
            displayName: '&eYeşil Yün'
        72:
            material: WOOL
            damage: 14
            displayName: '&eKırmızı Yün'
        73:
            material: WOOL
            damage: 15
            displayName: '&eSiyah Yün'
        75:
            material: GLASS
            displayName: '&eCam'
        76:
            material: STAINED_GLASS
            damage: 0
            displayName: '&eBeyaz Cam'
        77:
            material: STAINED_GLASS
            damage: 1
            displayName: '&eTuruncu Cam'
        78:
            material: STAINED_GLASS
            damage: 2
            displayName: '&eEflatun Cam'
        79:
            material: STAINED_GLASS
            damage: 3
            displayName: '&eAçık Mavi Cam'
        80:
            material: STAINED_GLASS
            damage: 4
            displayName: '&eSarı Cam'
        81:
            material: STAINED_GLASS
            damage: 5
            displayName: '&eAçık Yeşil Cam'
        82:
            material: STAINED_GLASS
            damage: 6
            displayName: '&ePembe Cam'
        83:
            material: STAINED_GLASS
            damage: 7
            displayName: '&eGri Cam'
        84:
            material: STAINED_GLASS
            damage: 8
            displayName: '&eAçık Gri Cam'
        85:
            material: STAINED_GLASS
            damage: 9
            displayName: '&eCamgöbeği Cam'
        86:
            material: STAINED_GLASS
            damage: 10
            displayName: '&eMor Cam'
        87:
            material: STAINED_GLASS
            damage: 11
            displayName: '&eMavi Cam'
        88:
            material: STAINED_GLASS
            damage: 12
            displayName: '&eKahverengi Cam'
        89:
            material: STAINED_GLASS
            damage: 13
            displayName: '&eYeşil Cam'
        90:
            material: STAINED_GLASS
            damage: 14
            displayName: '&eKırmızı Cam'
        91:
            material: STAINED_GLASS
            damage: 15
            displayName: '&eSiyah Cam'
    Dekor:
        slot: 13
        displayName: '&6Dekorasyon'
        material: BANNER
        displayLore:
        - ''
        - ' &8▪ &7Bu kategoride, ihtiyacın'
        - ' &7olan &edekorasyon ürünlerini'
        - ' &7inceleyebilir ve satın'
        - ' &7alabilirsin.'
        - ''
        - ' &8▸ &aTıkla ve alışverişe başla!'
        items:
        92:
            material: FENCE
            displayName: '&eMeşe Çiti'
        93:
            material: SPRUCE_FENCE
            displayName: '&eLadin Çiti'
        94:
            material: BIRCH_FENCE
            displayName: '&eHuş Çiti'
        95:
            material: JUNGLE_FENCE
            displayName: '&eOrman Çiti'
        96:
            material: ACACIA_FENCE
            displayName: '&eAkasya Çiti'
        97:
            material: DARK_OAK_FENCE
            displayName: '&eKoyu Meşe Çiti'
        98:
            material: COBBLE_WALL
            damage: 0
            displayName: '&eKırıktaş Duvar'
        99:
            material: COBBLE_WALL
            damage: 1
            displayName: '&eYosunlu Kırıktaş Duvar'
        100:
            material: IRON_FENCE
            displayName: '&eDemir Parmaklık'
        101:
            material: FENCE_GATE
            displayName: '&eMeşe Çit Kapısı'
        102:
            material: SPRUCE_FENCE_GATE
            displayName: '&eLadin Çit Kapısı'
        103:
            material: BIRCH_FENCE_GATE
            displayName: '&eHuş Çit Kapısı'
        104:
            material: JUNGLE_FENCE_GATE
            displayName: '&eOrman Çit Kapısı'
        105:
            material: ACACIA_FENCE_GATE
            displayName: '&eAkasya Çit Kapısı'
        106:
            material: DARK_OAK_FENCE_GATE
            displayName: '&eKoyu Meşe Çit Kapısı'
        107:
            material: FLOWER_POT_ITEM
            displayName: '&eSaksi'
        108:
            material: ARMOR_STAND
            displayName: '&eZırh Askısı'
        109:
            material: PAINTING
            displayName: '&eTablo'
        110:
            material: BANNER
            damage: 0
            displayName: '&eBeyaz Flama'
        111:
            material: BANNER
            damage: 1
            displayName: '&eTuruncu Flama'
        112:
            material: BANNER
            damage: 2
            displayName: '&eEflatun Flama'
        113:
            material: BANNER
            damage: 3
            displayName: '&eAçık Mavi Flama'
        114:
            material: BANNER
            damage: 4
            displayName: '&eSarı Flama'
        115:
            material: BANNER
            damage: 5
            displayName: '&eAçık Yeşil Flama'
        116:
            material: BANNER
            damage: 6
            displayName: '&ePembe Flama'
        117:
            material: BANNER
            damage: 7
            displayName: '&eGri Flama'
        118:
            material: BANNER
            damage: 8
            displayName: '&eAçık Gri Flama'
        119:
            material: BANNER
            damage: 9
            displayName: '&eCamgöbeği Flama'
        120:
            material: BANNER
            damage: 10
            displayName: '&eMor Flama'
        121:
            material: BANNER
            damage: 11
            displayName: '&eMavi Flama'
        122:
            material: BANNER
            damage: 12
            displayName: '&eKahverengi Flama'
        123:
            material: BANNER
            damage: 13
            displayName: '&eYeşil Flama'
        124:
            material: BANNER
            damage: 14
            displayName: '&eKırmızı Flama'
        125:
            material: BANNER
            damage: 15
            displayName: '&eSiyah Flama'
        126:
            material: THIN_GLASS
            displayName: '&eInce Cam'
        127:
            material: STAINED_GLASS_PANE
            damage: 0
            displayName: '&eBeyaz Ince Cam'
        128:
            material: STAINED_GLASS_PANE
            damage: 1
            displayName: '&eTuruncu Ince Cam'
        129:
            material: STAINED_GLASS_PANE
            damage: 2
            displayName: '&eEflatun Ince Cam'
        130:
            material: STAINED_GLASS_PANE
            damage: 3
            displayName: '&eAçık Mavi Ince Cam'
        131:
            material: STAINED_GLASS_PANE
            damage: 4
            displayName: '&eSarı Ince Cam'
        132:
            material: STAINED_GLASS_PANE
            damage: 5
            displayName: '&eAçık Yeşil Ince Cam'
        133:
            material: STAINED_GLASS_PANE
            damage: 6
            displayName: '&ePembe Ince Cam'
        134:
            material: STAINED_GLASS_PANE
            damage: 7
            displayName: '&eGri Ince Cam'
        135:
            material: STAINED_GLASS_PANE
            damage: 8
            displayName: '&eAçık Gri Ince Cam'
        136:
            material: STAINED_GLASS_PANE
            damage: 9
            displayName: '&eCamgöbeği Ince Cam'
        137:
            material: STAINED_GLASS_PANE
            damage: 10
            displayName: '&eMor Ince Cam'
        138:
            material: STAINED_GLASS_PANE
            damage: 11
            displayName: '&eMavi Ince Cam'
        139:
            material: STAINED_GLASS_PANE
            damage: 12
            displayName: '&eKahverengi Ince Cam'
        140:
            material: STAINED_GLASS_PANE
            damage: 13
            displayName: '&eYeşil Ince Cam'
        141:
            material: STAINED_GLASS_PANE
            damage: 14
            displayName: '&eKırmızı Ince Cam'
        142:
            material: STAINED_GLASS_PANE
            damage: 15
            displayName: '&eSiyah Ince Cam'
        143:
            material: CARPET
            damage: 0
            displayName: '&eBeyaz Halı'
        144:
            material: CARPET
            damage: 1
            displayName: '&eTuruncu Halı'
        145:
            material: CARPET
            damage: 2
            displayName: '&eEflatun Halı'
        146:
            material: CARPET
            damage: 3
            displayName: '&eAçık Mavi Halı'
        147:
            material: CARPET
            damage: 4
            displayName: '&eSarı Halı'
        148:
            material: CARPET
            damage: 5
            displayName: '&eAçık Yeşil Halı'
        149:
            material: CARPET
            damage: 6
            displayName: '&ePembe Halı'
        150:
            material: CARPET
            damage: 7
            displayName: '&eGri Halı'
        151:
            material: CARPET
            damage: 8
            displayName: '&eAçık Gri Halı'
        152:
            material: CARPET
            damage: 9
            displayName: '&eCamgöbeği Halı'
        153:
            material: CARPET
            damage: 10
            displayName: '&eMor Halı'
        154:
            material: CARPET
            damage: 11
            displayName: '&eMavi Halı'
        155:
            material: CARPET
            damage: 12
            displayName: '&eKahverengi Halı'
        156:
            material: CARPET
            damage: 13
            displayName: '&eYeşil Halı'
        157:
            material: CARPET
            damage: 14
            displayName: '&eKırmızı Halı'
        158:
            material: CARPET
            damage: 15
            displayName: '&eSiyah Halı'
    KızılT:
        slot: 14
        displayName: '&6Kızıltaş ve Ulaşım'
        material: REDSTONE
        displayLore:
        - ''
        - ' &8▪ &7Bu kategoride, ihtiyacın'
        - ' &7olan &ekızıltaş ürünlerini'
        - ' &7inceleyebilir ve satın'
        - ' &7alabilirsin.'
        - ''
        - ' &8▸ &aTıkla ve alışverişe başla!'
        items:
        159:
            material: NOTE_BLOCK
            displayName: '&eNota Bloğu'
        160:
            material: PISTON_BASE
            displayName: '&ePiston'
        161:
            material: REDSTONE_LAMP_OFF
            displayName: '&eKızıltaş Lambası'
        162:
            material: DAYLIGHT_DETECTOR
            displayName: '&eGüneş Sensörü'
        163:
            material: REDSTONE
            displayName: '&eKızıltaş'
        164:
            material: REDSTONE_BLOCK
            displayName: '&eKızıltaş Bloğu'
        165:
            material: HOPPER
            displayName: '&eHuni'
        166:
            material: DIODE
            displayName: '&eKızıltaş Yineleyici'
        167:
            material: REDSTONE_COMPARATOR
            displayName: '&eKızıltaş Karşılaştırıcı'
        168:
            material: WOOD_DOOR
            displayName: '&eMeşe Kapı'
        169:
            material: IRON_DOOR
            displayName: '&eDemir Kapı'
        170:
            material: SPRUCE_DOOR_ITEM
            displayName: '&eLadin Kapı'
        171:
            material: BIRCH_DOOR_ITEM
            displayName: '&eHuş Kapı'
        172:
            material: JUNGLE_DOOR_ITEM
            displayName: '&eOrman Kapı'
        173:
            material: ACACIA_DOOR_ITEM
            displayName: '&eAkasya Kapı'
        174:
            material: DARK_OAK_DOOR_ITEM
            displayName: '&eKoyu Meşe Kapı'
        175:
            material: POWERED_RAIL
            displayName: '&eGüçlendirilmiş Ray'
        176:
            material: DETECTOR_RAIL
            displayName: '&eDedektör Ray'
        177:
            material: ACTIVATOR_RAIL
            displayName: '&eAktivatör Ray'
        178:
            material: RAILS
            displayName: '&eRay'
        179:
            material: MINECART
            displayName: '&eMinecart'
        180:
            material: STORAGE_MINECART
            displayName: '&eSandıklı Vagon'
        181:
            material: HOPPER_MINECART
            displayName: '&eHunili Vagon'
        182:
            material: POWERED_MINECART
            displayName: '&eFırınlı Vagon'
        183:
            material: DISPENSER
            displayName: '&eFırlatıcı'
        184:
            material: DROPPER
            displayName: '&eBırakıcı'
        185:
            material: SADDLE
            displayName: '&eEyer'
        186:
            material: BOAT
            displayName: '&eTekne'
        187:
            material: CARROT_STICK
            displayName: '&eHavuçlu Olta'
    Iksir:
        slot: 15
        displayName: '&6Iksir'
        material: BREWING_STAND_ITEM
        displayLore:
        - ''
        - ' &8▪ &7Bu kategoride, ihtiyacın'
        - ' &7olan &eiksirleri &7inceleyebilir'
        - ' &7ve satın alabilirsin.'
        - ''
        - ' &8▸ &aTıkla ve alışverişe başla!'
        items:
        188:
            material: POTION
            damage: 0
            displayName: '&eSu Şişesi'
        189:
            material: GLASS_BOTTLE
            displayName: '&eCam Şişe'
        190:
            material: GHAST_TEAR
            displayName: '&eGhast Gözyaşı'
        191:
            material: FERMENTED_SPIDER_EYE
            displayName: '&eMayalı Örümcek Gözü'
        192:
            material: BLAZE_POWDER
            displayName: '&eBlaze Tozu'
        193:
            material: MAGMA_CREAM
            displayName: '&eMagma Kremi'
        194:
            material: SPECKLED_MELON
            displayName: '&eParlayan Karpuz'
        195:
            material: GOLDEN_CARROT
            displayName: '&eAltın Havuç'
        196:
            material: RABBIT_FOOT
            displayName: '&eTavşan Ayağı'
        197:
            material: SULPHUR
            displayName: '&eBarut'
        198:
            material: GLOWSTONE_DUST
            displayName: '&eIşıktaşı Tozu'
        199:
            material: SUGAR
            displayName: '&eŞeker'
        200:
            material: BLAZE_ROD
            displayName: '&eBlaze Çubuğu'
        201:
            material: NETHER_STALK
            displayName: '&eNetherwart'
        202:
            material: BREWING_STAND_ITEM
            displayName: '&eSimya Standı'
        203:
            material: CAULDRON_ITEM
            displayName: '&eKazan'
        204:
            material: POTION
            damage: 8193
            displayName: '&eRejenerasyon Iksiri'
        205:
            material: POTION
            damage: 8225
            displayName: '&eRejenerasyon Iksiri'
        206:
            material: POTION
            damage: 8257
            displayName: '&eRejenerasyon Iksiri'
        207:
            material: POTION
            damage: 8194
            displayName: '&eÇeviklik Iksiri'
        208:
            material: POTION
            damage: 8226
            displayName: '&eÇeviklik Iksiri'
        209:
            material: POTION
            damage: 8258
            displayName: '&eÇeviklik Iksiri'
        210:
            material: POTION
            damage: 8227
            displayName: '&eAteş Direnci Iksiri'
        211:
            material: POTION
            damage: 8259
            displayName: '&eAteş Direnci Iksiri'
        212:
            material: POTION
            damage: 8196
            displayName: '&eZehir Iksiri'
        213:
            material: POTION
            damage: 8228
            displayName: '&eZehir Iksiri'
        214:
            material: POTION
            damage: 8260
            displayName: '&eZehir Iksiri'
        215:
            material: POTION
            damage: 8261
            displayName: '&eIyileştirme Iksiri'
        216:
            material: POTION
            damage: 8229
            displayName: '&eIyileştirme Iksiri'
        217:
            material: POTION
            damage: 8230
            displayName: '&eGece Görüşü Iksiri'
        218:
            material: POTION
            damage: 8262
            displayName: '&eGece Görüşü Iksiri'
        219:
            material: POTION
            damage: 8232
            displayName: '&eZayıflık Iksiri'
        220:
            material: POTION
            damage: 8264
            displayName: '&eZayıflık Iksiri'
        221:
            material: POTION
            damage: 8201
            displayName: '&eGüç Iksiri'
        222:
            material: POTION
            damage: 8233
            displayName: '&eGüç Iksiri'
        223:
            material: POTION
            damage: 8265
            displayName: '&eGüç Iksiri'
        224:
            material: POTION
            damage: 8234
            displayName: '&eYavaşlatma Iksiri'
        225:
            material: POTION
            damage: 8266
            displayName: '&eYavaşlatma Iksiri'
        226:
            material: POTION
            damage: 8203
            displayName: '&eSıçrama Iksiri'
        227:
            material: POTION
            damage: 8235
            displayName: '&eSıçrama Iksiri'
        228:
            material: POTION
            damage: 8267
            displayName: '&eSıçrama Iksiri'
        229:
            material: POTION
            damage: 8237
            displayName: '&eSualtı Iksiri'
        230:
            material: POTION
            damage: 8269
            displayName: '&eSualtı Iksiri'
        231:
            material: POTION
            damage: 16385
            displayName: '&ePatlayıcı Rejenerasyon Iksiri'
        232:
            material: POTION
            damage: 16417
            displayName: '&ePatlayıcı Rejenerasyon Iksiri'
        233:
            material: POTION
            damage: 16449
            displayName: '&ePatlayıcı Rejenerasyon Iksiri'
        234:
            material: POTION
            damage: 16386
            displayName: '&ePatlayıcı Hız Iksiri'
        235:
            material: POTION
            damage: 16418
            displayName: '&ePatlayıcı Hız Iksiri'
        236:
            material: POTION
            damage: 16450
            displayName: '&ePatlayıcı Hız Iksiri'
        237:
            material: POTION
            damage: 16419
            displayName: '&ePatlayıcı Ateş Direnci Iksiri'
        238:
            material: POTION
            damage: 16451
            displayName: '&ePatlayıcı Ateş Direnci Iksiri'
        239:
            material: POTION
            damage: 16388
            displayName: '&ePatlayıcı Zehir Iksiri'
        240:
            material: POTION
            damage: 16420
            displayName: '&ePatlayıcı Zehir Iksiri'
        241:
            material: POTION
            damage: 16452
            displayName: '&ePatlayıcı Zehir Iksiri'
        242:
            material: POTION
            damage: 16453
            displayName: '&ePatlayıcı Iyileştirme Iksiri'
        243:
            material: POTION
            damage: 16421
            displayName: '&ePatlayıcı Iyileştirme Iksiri'
        244:
            material: POTION
            damage: 16422
            displayName: '&ePatlayıcı Gece Görüş Iksiri'
        245:
            material: POTION
            damage: 16454
            displayName: '&ePatlayıcı Gece Görüş Iksiri'
        246:
            material: POTION
            damage: 16424
            displayName: '&ePatlayıcı Zayıflık Iksiri'
        247:
            material: POTION
            damage: 16456
            displayName: '&ePatlayıcı Zayıflık Iksiri'
        248:
            material: POTION
            damage: 16393
            displayName: '&ePatlayıcı Güç Iksiri'
        249:
            material: POTION
            damage: 16425
            displayName: '&ePatlayıcı Güç Iksiri'
        250:
            material: POTION
            damage: 16457
            displayName: '&ePatlayıcı Güç Iksiri'
        251:
            material: POTION
            damage: 16426
            displayName: '&ePatlayıcı Yavaşlık Iksiri'
        252:
            material: POTION
            damage: 16458
            displayName: '&ePatlayıcı Yavaşlık Iksiri'
        253:
            material: POTION
            damage: 16395
            displayName: '&ePatlayıcı Sıçrama Iksiri'
        254:
            material: POTION
            damage: 16427
            displayName: '&ePatlayıcı Sıçrama Iksiri'
        255:
            material: POTION
            damage: 16459
            displayName: '&ePatlayıcı Sıçrama Iksiri'
        256:
            material: POTION
            damage: 16460
            displayName: '&ePatlayıcı Zarar Iksiri'
        257:
            material: POTION
            damage: 16428
            displayName: '&ePatlayıcı Zarar Iksiri'
        258:
            material: POTION
            damage: 16461
            displayName: '&ePatlayıcı Sualtı Iksiri'
    Malzeme:
        slot: 21
        displayName: '&6Malzemeler'
        material: DIAMOND
        displayLore:
        - ''
        - ' &8▪ &7Bu kategoride, ihtiyacın'
        - ' &7olan &ecevher, boya &7gibi'
        - ' &7ürünleri inceleyebilir ve'
        - ' &7satın alabilirsin.'
        - ''
        - ' &8▸ &aTıkla ve alışverişe başla!'
        items:
        259:
            material: EMERALD
            displayName: '&eZümrüt'
        260:
            material: DIAMOND
            displayName: '&eElmas'
        261:
            material: IRON_INGOT
            displayName: '&eDemir'
        262:
            material: GOLD_INGOT
            displayName: '&eAltın'
        263:
            material: COAL
            damage: 0
            displayName: '&eKömür'
        264:
            material: COAL
            damage: 1
            displayName: '&eOdun Kömürü'
        265:
            material: NETHER_BRICK_ITEM
            displayName: '&eNether Tuğlası'
        266:
            material: STICK
            displayName: '&eÇubuk'
        267:
            material: BOWL
            displayName: '&eKase'
        268:
            material: STRING
            displayName: '&eIp'
        269:
            material: FEATHER
            displayName: '&eTüy'
        270:
            material: FLINT
            displayName: '&eÇakmaktaşı'
        271:
            material: LEATHER
            displayName: '&eDeri'
        272:
            material: CLAY_BALL
            displayName: '&eKil'
        273:
            material: SUGAR_CANE
            displayName: '&eŞeker Kamışı'
        274:
            material: NETHER_STAR
            displayName: '&eNether Yıldızı'
        275:
            material: RABBIT_HIDE
            displayName: '&eTavşan Postu'
        276:
            material: QUARTZ
            displayName: '&eKuvars'
        277:
            material: INK_SACK
            damage: 0
            displayName: '&eMürekkep Kesesi'
        278:
            material: INK_SACK
            damage: 1
            displayName: '&eGül Kırmızısı'
        279:
            material: INK_SACK
            damage: 2
            displayName: '&eKaktüs Yeşili'
        280:
            material: INK_SACK
            damage: 3
            displayName: '&eKakao Çekirdekleri'
        281:
            material: INK_SACK
            damage: 4
            displayName: '&eLapis Lazuli'
        282:
            material: INK_SACK
            damage: 5
            displayName: '&eMor Boya'
        283:
            material: INK_SACK
            damage: 6
            displayName: '&eCamgöbeği Boya'
        284:
            material: INK_SACK
            damage: 7
            displayName: '&eAçık Gri Boya'
        285:
            material: INK_SACK
            damage: 8
            displayName: '&eGri Boya'
        286:
            material: INK_SACK
            damage: 9
            displayName: '&ePembe Boya'
        287:
            material: INK_SACK
            damage: 10
            displayName: '&eKireç Boya'
        288:
            material: INK_SACK
            damage: 11
            displayName: '&eKarahindiba Sarısı'
        289:
            material: INK_SACK
            damage: 12
            displayName: '&eAçık Mavi Boya'
        367:
            material: INK_SACK
            damage: 13
            displayName: '&eEflatun Boya'
        368:
            material: INK_SACK
            damage: 14
            displayName: '&eTuruncu Boya'
        369:
            material: INK_SACK
            damage: 15
            displayName: '&eKemik Tozu'
    Yemek:
        slot: 22
        displayName: '&6Yemek'
        material: APPLE
        displayLore:
        - ''
        - ' &8▪ &7Bu kategoride, ihtiyacın'
        - ' &7olan &eyemekleri &7inceleyebilir'
        - ' &7ve satın alabilirsin.'
        - ''
        - ' &8▸ &aTıkla ve alışverişe başla!'
        items:
        370:
            material: GOLDEN_APPLE
            damage: 0
            displayName: '&eAltın Elma'
        371:
            material: GOLDEN_APPLE
            damage: 1
            displayName: '&eBüyülü Altın Elma'
        372:
            material: APPLE
            displayName: '&eElma'
        373:
            material: MUSHROOM_SOUP
            displayName: '&eMantar Güveç'
        374:
            material: BREAD
            displayName: '&eEkmek'
        375:
            material: PORK
            displayName: '&eÇiğ Domuz Eti'
        376:
            material: GRILLED_PORK
            displayName: '&eDomuz Eti'
        377:
            material: RAW_FISH
            damage: 0
            displayName: '&eÇiğ Balık'
        378:
            material: RAW_FISH
            damage: 1
            displayName: '&eÇiğ Somon Balığı'
        379:
            material: RAW_FISH
            damage: 2
            displayName: '&ePalyaço Balığı'
        380:
            material: RAW_FISH
            damage: 3
            displayName: '&eKirpi Balığı'
        381:
            material: COOKED_FISH
            damage: 0
            displayName: '&ePişmiş Balık'
        382:
            material: COOKED_FISH
            damage: 1
            displayName: '&ePişmiş Somon Balık'
        392:
            material: CAKE
            displayName: '&ePasta'
        393:
            material: COOKIE
            displayName: '&eKurabiye'
        394:
            material: MELON
            displayName: '&eKarpuz'
        395:
            material: RAW_BEEF
            displayName: '&eÇiğ Biftek'
        396:
            material: COOKED_BEEF
            displayName: '&eBiftek'
        397:
            material: RAW_CHICKEN
            displayName: '&eÇiğ Tavuk Eti'
        398:
            material: COOKED_CHICKEN
            displayName: '&ePişmiş Tavuk Eti'
        399:
            material: CARROT_ITEM
            displayName: '&eHavuç'
        400:
            material: POTATO_ITEM
            displayName: '&ePatates'
        401:
            material: BAKED_POTATO
            displayName: '&eHaşlanmış Patates'
        402:
            material: PUMPKIN_PIE
            displayName: '&eBalkabağı Turtası'
        403:
            material: RABBIT
            displayName: '&eÇiğ Tavşan Eti'
        404:
            material: COOKED_RABBIT
            displayName: '&ePişmiş Tavşan Eti'
        405:
            material: RABBIT_STEW
            displayName: '&eTavşan Yahnisi'
        406:
            material: MUTTON
            displayName: '&eÇiğ Koyun Eti'
        407:
            material: COOKED_MUTTON
            displayName: '&ePişmiş Koyun Eti'
    Kitap:
        slot: 23
        displayName: '&6Büyülü Kitaplar'
        material: ENCHANTED_BOOK
        displayLore:
        - ''
        - ' &8▪ &7Bu kategoride, ihtiyacın'
        - ' &7olan &ebüyülü kitapları'
        - ' &7inceleyebilir ve satın'
        - ' &7alabilirsin.'
        - ''
        - ' &8▸ &aTıkla ve alışverişe başla!'
        items:
        408:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_ENVIRONMENTAL:1
        409:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_ENVIRONMENTAL:2
        410:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_ENVIRONMENTAL:3
        411:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_ENVIRONMENTAL:4
        412:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_FIRE:1
        413:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_FIRE:2
        414:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_FIRE:3
        415:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_FIREL:4
        416:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_FALL:1
        417:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_FALL:2
        418:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_FALL:3
        419:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_FALL:4
        420:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_EXPLOSIONS:1
        421:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_EXPLOSIONS:2
        422:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_EXPLOSIONS:3
        423:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_EXPLOSIONS:4
        424:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_PROJECTILE:1
        425:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_PROJECTILE:2
        426:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_PROJECTILE:3
        427:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - PROTECTION_PROJECTILE:4
        428:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - OXYGEN:1
        429:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - OXYGEN:2
        430:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - OXYGEN:3
        431:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - WATER_WORKER:1
        432:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - THORNS:1
        433:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - THORNS:2
        444:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - THORNS:3
        435:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DEPTH_STRIDER:1
        290:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DEPTH_STRIDER:2
        291:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DEPTH_STRIDER:3
        292:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DAMAGE_ALL:1
        293:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DAMAGE_ALL:2
        294:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DAMAGE_ALL:3
        295:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DAMAGE_ALL:4
        296:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DAMAGE_ALL:5
        297:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DAMAGE_UNDEAD:1
        298:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DAMAGE_UNDEAD:2
        299:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DAMAGE_UNDEAD:3
        300:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DAMAGE_UNDEAD:4
        301:
            material: ENCHANTED_BOOK
            ddisplayName: '&eBüyülü Kitap'
            enchantment:
            - DAMAGE_UNDEAD:5
        302:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DAMAGE_ARTHROPODS:1
        303:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DAMAGE_ARTHROPODS:2
        304:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DAMAGE_ARTHROPODS:3
        305:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DAMAGE_ARTHROPODS:4
        306:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DAMAGE_ARTHROPODS:5
        307:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - KNOCKBACK:1
        308:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - KNOCKBACK:2
        309:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - FIRE_ASPECT:1
        310:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - FIRE_ASPECT:2
        311:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - LOOT_BONUS_MOBS:1
        312:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - LOOT_BONUS_MOBS:2
        313:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - LOOT_BONUS_MOBS:3
        314:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DIG_SPEED:1
        315:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DIG_SPEED:2
        316:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DIG_SPEED:3
        317:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DIG_SPEED:4
        318:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DIG_SPEED:5
        319:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - SILK_TOUCH:1
        320:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DURABILITY:1
        321:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DURABILITY:2
        322:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DURABILITY:3
        323:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DURABILITY:4
        324:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - DURABILITY:5
        325:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - LOOT_BONUS_BLOCKS:1
        326:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - LOOT_BONUS_BLOCKS:2
        327:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - LOOT_BONUS_BLOCKS:3
        328:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - ARROW_DAMAGE:1
        329:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - ARROW_DAMAGE:2
        330:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - ARROW_DAMAGE:3
        331:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - ARROW_DAMAGE:4
        332:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - ARROW_DAMAGE:5
        333:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - ARROW_KNOCKBACK:1
        334:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - ARROW_KNOCKBACK:2
        335:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - ARROW_FIRE:1
        336:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - ARROW_INFINITE:1
        337:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - LUCK:1
        338:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - LUCK:2
        339:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - LUCK:3
        340:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - LURE:1
        341:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - LURE:2
        342:
            material: ENCHANTED_BOOK
            displayName: '&eBüyülü Kitap'
            enchantment:
            - LURE:3
    Diğer:
        slot: 24
        displayName: '&6Diğer'
        material: LAVA_BUCKET
        displayLore:
        - ''
        - ' &8▪ &7Bu kategoride, ihtiyacın'
        - ' &7olan &ekayış, kova, makas &7gibi'
        - ' &7çeşitli ürünleri inceleyebilir'
        - ' &7ve satın alabilirsin.'
        - ''
        - ' &8▸ &aTıkla ve alışverişe başla!'
        items:
        343:
            material: ENCHANTMENT_TABLE
            displayName: '&eBüyü Masası'
        344:
            material: BUCKET
            displayName: '&eKova'
        345:
            material: LAVA_BUCKET
            displayName: '&eLav Kovası'
        346:
            material: WATER_BUCKET
            displayName: '&eSu Kovası'
        347:
            material: MILK_BUCKET
            displayName: '&eSüt Kovası'
        348:
            material: ENDER_PEARL
            displayName: '&eEnder Incisi'
        349:
            material: EYE_OF_ENDER
            displayName: '&eEnder Gözü'
        350:
            material: IRON_BARDING
            displayName: '&eDemir At Zırhı'
        351:
            material: GOLD_BARDING
            displayName: '&eAltın At Zırhı'
        352:
            material: DIAMOND_BARDING
            displayName: '&eElmas At Zırhı'
        353:
            material: FISHING_ROD
            displayName: '&eOlta'
        354:
            material: WATCH
            displayName: '&eSaat'
        355:
            material: SHEARS
            displayName: '&eMakas'
        356:
            material: NAME_TAG
            displayName: '&eIsim Etiketi'
        357:
            material: FLINT_AND_STEEL
            displayName: '&eÇakmaktaşı ve Çelik'
        358:
            material: BOW
            displayName: '&eYay'
        359:
            material: ARROW
            displayName: '&eOk'
        360:
            material: LADDER
            displayName: '&eMerdiven'
        361:
            material: TORCH
            displayName: '&eMeşale'
        362:
            material: SIGN
            displayName: '&eTabela'
        363:
            material: ITEM_FRAME
            displayName: '&eEşya Çerçevesi'
        364:
            material: SLIME_BALL
            displayName: '&eBalçık Topu'
        365:
            material: SKULL_ITEM
            damage: 1
            displayName: '&eWither Kafası'
        366:
            material: LEASH
            displayName: '&eKayış'       
    confirmation:
    yesItem:
        slot: 11
        material: stained_clay
        damage: 5
        name: '&aKabul Et'
        lore:
        - ''
        - ' &8▪ &7İşlemi onayla!'
    noItem:
        slot: 15
        material: stained_clay
        damage: 14
        name: '&4Reddet'
        lore:
        - ''
        - ' &8▪ &7İşlemi iptal et!'
    fill:
        material: stained_glass_pane
        damage: 7
</details>

<details>
    <summary>lang.yml</summary>
        TuccarGui: '&8Tüccar'
        CategoryGui: '&8Tüccar &0/'
        itemGui: '&8Ürünler &0/'
        confirmationGui: '&aOnaylama'
        selfProducts: '&6Ürünlerim'
        Messages:
        productSold: ' &6Tüccar &8▸ &2{product}x{amount} &asatıldı. &2+{price}'
        listItem: ' &6Tüccar &8▸ &7Ürün başarıyla listelendi!'
        dontHavePerm: ' &6Tüccar &8▸ &cBunun için yetkin yok!'
        inputMustInteger: '&6Tüccar &8▸ &cFiyat sayı olmalıdır!'
        notEnoughItem: ' &6Tüccar &8▸ &cYeterli sayıda ürün bulunamadı!'
        couldntFindStock: ' &6Tüccar &8▸ &cStok bulunamadı!'
        notInAllowedWorld: ' &6Tüccar &8▸ &cBunun için doğru dünyada değilsin!'
        priceLow: ' &6Tüccar &8▸ &cFiyat &4{min} &cdan düşük olamaz!'
        rePrice: ' &6Tüccar &8▸ &aÜrünün fiyatını güncellemek için sohbete fiyatı 10 saniye içinde yaz.'
        rePriceSuccess: ' &6Tüccar &8▸ &aYeniden fiyat ayarlaması tamamlandı.'
        cannotBuyOwnItem: ' &6Tüccar &8▸ &cKendi ürününü satın alamazsın!'
        couldntFindItem: ' &6Tüccar &8▸ &cBöyle bir ürün bulunamadı!'
        setNpcSuccess: ' &6Tüccar &8▸ &aTüccar NPCsi &2başarıyla &akondu.'
        reload: ' &6Tüccar &8▸ &aYenileme işlemi &2başarıyla &agerçekleştirildi.'
        help:
        - ''
        - '&6 TÜCCAR SİSTEMİ:'
        - ''
        - '&6 /tüccar ekle &d[Birim Fiyatı] <Stok Sayısı/El/Hepsi> &8▸ &7Tüccara ürün kayıt eder.'
        - '&6 /tüccar stokekle &d<Stok Sayısı/El/Hepsi> &8▸ &7Tüccara stok ekler.'
        - '&6 /tüccar ürünlerim &8▸ &7Tüccardaki ürünlerini gösterir.'
        - ''
        - '&7 Tüccar menüsünden ürünlerini &Ciptal edip&7/&adüzenleyebilirsin.'
        - '&d<değer> &8▸ &7Opsiyonel &8(zorunlu olmayan) &7verilerdir.'
        - '&d[değer] &8▸ &cZorunlu &7girilmesi gereken verilerdir.'
        Titles:
        processCancelled:
            title: '&4Onay'
            subTitle: '&cOnay verilmedi!'
        processSuccess:
            title: '&2Onay'
            subTitle: '&aOnay alındı!'
        errorConfirmation:
            title: '&4Hata'
            subTitle: '&cSatın alınamadı.'
        notEnoughSpace:
            title: '&4Hata'
            subTitle: '&cEnvanter dolu.'
        notEnoughMoney:
            title: '&4Hata'
            subTitle: '&cYeterli para yok.'
        Gui:
        myProducts:
            slot: 19
            material: CHEST
            name: '&6Ürünlerim'
            lore:
            - ''
            - '&8▪ &7Buradan daha önce tüccara'
            - '&7eklemiş olduğun ürünleri görebilirsin.'
        itemCategoryTemplate:
        - ''
        - '&8▪ &7Satıcı Sayısı: &e{seller_amount}'
        - '&8▪ &7Minimum Fiyat: &e{min_price}'
        - ''
        cancelTemplate:
        - ''
        - ' &8▪ &7Kategori: &a{category}'
        - ' &8▪ &7Adet: &a{amount}'
        - ' &8▪ &7Satıcı: &c{seller}'
        - ' &8▪ &7Fiyat: &6{price}'
        - ''
        filter:
            material: HOPPER
            name: '&6Filtreleyici'
            lore:
            - ''
            - '&8▪ &7Satışı olmayan ürünleri filtreler.'
            - '&8▪ &7Mevcut durum: &a{filter_status}'
        empty:
            material: BARRIER
            name: '&4Sekme Boş'
            lore:
            - ''
            - '&7▪ Bu menü boş görünüyor!'
        nextPage:
            material: ARROW
            name: '&eSonraki Sayfa'
            lore:
            - ''
            - '&8▪ &7Sonraki sayfaya geç!'
        previousPage:
            material: ARROW
            name: '&eÖnceki Sayfa'
            lore:
            - ''
            - '&8▪ &7Önceki sayfaya dön!'
        backToMenu:
            material: ARROW
            name: '&cGeri Dön'
            lore:
            - ''
            - '&8▪ &7Önceki menüye dön!'
        help:
            slot: 10
            material: BOOK
            name: '&6Bilgi'
            lore:
            - ''
            - '&8▪ &7Tüccar eşyalarını satışa çıkarır'
            - '&7Ve buradan yaptığın satışlar ile'
            - '&7Para kazanabilirsin!'
        selfProductHelp:
            slot: 45
            material: BOOK
            name: '&6Bilgi'
            lore:
            - ''
            - '&8▪ &7Burada kendi sattığın ürünleri'
            - '&7Görebilirsin ve onları iptal edebilirsin.'
        selfProductTemplate:
            lore:
            - ''
            - ' &8▪ &7Stok: &a{stock}'
            - ' &8▪ &7Fiyat: &a{price}'
            - ' &8▪ &7Kategori: &a{category}'
            - ''
            - '&e1 Adet iptal etmek için &6[Sol Tık]'
        #    - "&e{custom_amount} Adet iptal etmek için &6[Shift + Sol Tık]"
            - '&e1 Stack iptal etmek için &6[Sağ Tık]'
            - '&eHepsini iptal etmek için &6[Shift + Sağ Tık]'
            - '&eFiyatı güncellemek için &6[Orta Tık]'
        itemTemplate:
            lore:
            - ''
            - ' &8▪ &7Satıcı: &a{seller}'
            - ' &8▪ &7Stok: &a{stock}'
            - ' &8▪ &7Fiyat: &a{price}'
            - ''
            - '&e1 Adet satın almak için &6[Sol Tık]'
        #    - "&e{custom_amount} Adet satın almak için &6[Shift + Sol Tık]"
            - '&e1 Stack satın almak için &6[Sağ Tık]'
            - '&eEnvanterini doldurmak için &6[Shift + Sağ Tık]'
</details>

## Komutlar
+ **/tüccar** - Tüccar menüsünü açar
+ **/tüccar belirle** - Tüccar NPC'sini belirler (Citizens NPC'sine bakmak gerekir)
+ **/tüccar ekle** - Tüccar'a ürün ekler
+ **/tüccar stokekle** - Mevcut ürüne stok ekler
+ **/tüccar ürünlerim** - Oyuncunun tüccarda listelediği ürünleri listeler.
+ **/tüccar reload** - Config ve dil dosyasını yeniden yükler.

## Resimler
TODO

## Kullanılan Kütüphaneler

* [spigot-api (1.19-R0.3-SNAPSHOT)](https://hub.spigotmc.org/stash/projects/SPIGOT/repos/spigot/browse)
* [lombok (LATEST)](https://github.com/projectlombok/lombok)
* [BStats](https://bstats.org)
* [Vault](https://www.spigotmc.org/resources/vault.34315/)
* [JSON](https://mvnrepository.com/artifact/org.json/json)
* [Citizens](https://wiki.citizensnpcs.co/Citizens_Wiki)

## Contributing

We welcome contributions from the community! If you would like to contribute, please follow these guidelines:

1. Fork the repository and clone it to your local machine.
2. Create a new branch for your feature or bug fix.
3. Make your changes, and ensure that your code is well-tested.
4. Create a pull request with a detailed description of your changes.

By contributing to this project, you agree to abide by the [Code of Conduct](CODE_OF_CONDUCT.md).
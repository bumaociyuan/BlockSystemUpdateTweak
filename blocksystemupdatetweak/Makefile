THEOS_DEVICE_IP = localhost
THEOS_DEVICE_PORT = 2222
include $(THEOS)/makefiles/common.mk

TWEAK_NAME = BlockSystemUpdateTweak
BlockSystemUpdateTweak_FILES = Tweak.xm

include $(THEOS_MAKE_PATH)/tweak.mk

after-install::
	install.exec "killall -9 com.apple.Preferences"

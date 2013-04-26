OUTPUT_DIR = ../../assets/

#
# BUILD SIMPLE FOUNDATION DIRECTORY
#

foundation: foundation-css foundation-js


#
# JS COMPILE
#
foundation-js: foundation/js/foundation/*.js

foundation/js/foundation/*.js: js/foundation/*.js
	cat js/foundation/foundation.js js/foundation/foundation.alerts.js js/foundation/foundation.clearing.js js/foundation/foundation.cookie.js js/foundation/foundation.dropdown.js js/foundation/foundation.forms.js js/foundation/foundation.joyride.js js/foundation/foundation.magellan.js js/foundation/foundation.orbit.js js/foundation/foundation.placeholder.js js/foundation/foundation.reveal.js js/foundation/foundation.section.js js/foundation/foundation.tooltips.js js/foundation/foundation.topbar.js > ${OUTPUT_DIR}js/foundation.js
	cp js/vendor/*.js ${OUTPUT_DIR}js/vendor/


#
# CSS COMPLILE
# Sass & Compass are required
# Compass configuration in config.rb
#

foundation-css: foundation/scss/*.scss

foundation/scss/*.scss: scss/*.scss
	compass compile


.PHONY: foundation-css foundation-js
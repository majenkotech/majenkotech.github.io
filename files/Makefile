TFT_FILES = BMPFile gciWidget Hazard Liberation OCR_A Open24Display Raw565File TFT Widgets
TFT_ZIP = TFT-Complete.zip
FILES = ${TFT_FILES}

ZIPS = ${TFT_ZIP}

${TFT_ZIP}: pull ${TFT_FILES}
	zip -r ${TFT_ZIP} ${TFT_FILES} -x *.git*

pull:
	@for FILE in ${FILES}; do (cd $$FILE; echo -n $$FILE "... "; git pull); done

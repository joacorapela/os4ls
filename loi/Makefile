all: application.md

application.md: title.md summary.md expectedValue.md landscape.md
	echo "# Title (" `wc -c < title.md` "/ 60 words )" > application.md
	cat title.md >> application.md
	echo "\n# Summary (" `wc -c < summary.md` "/ 3000 words)" >> application.md
	cat summary.md >> application.md
	echo "\n# Expected Value (" `wc -c < expectedValue.md` "/ 1500 words)" >> application.md
	cat expectedValue.md >> application.md
	echo "\n# Landscape Analysis (" `wc -c < landscape.md` "/ 1500 words)" >> application.md
	cat landscape.md >> application.md

all: application.md

application.md: title.md summary.md expectedValue.md landscape.md
	echo "# Title (60 words)" > application.md
	cat title.md >> application.md
	echo "\n# Summary (3000 words)" >> application.md
	cat summary.md >> application.md
	echo "\n# Expected Value (1500 words)" >> application.md
	cat expectedValue.md >> application.md
	echo "\n# Landscape Analysis (1500 words)" >> application.md
	cat landscape.md >> application.md

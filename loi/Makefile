all: application.md

application.md: title.md summary.md expectedValue.md landscape.md
	echo "# Title (" `wc -c < title.md` "/ 60 words )" > application.md
	cat title.md >> application.md
	echo "\n# Summary (" `wc -c < summary.md` "/ 3000 words)" >> application.md
	echo "\nBriefly describe the purpose of the proposal and the software project(s) it involves." >> application.md
	cat summary.md >> application.md
	echo "\n# Expected Value (" `wc -c < expectedValue.md` "/ 1500 words)" >> application.md
	echo "\nIf the proposal is successfully funded, what does success look like? We're seeking to understand: what type of capabilities the proposal is unlocking for the scientific community; how upstream and downstream software will be improved by the proposal; how the proposed work supports or implements novel functionality for AI enablement and large-scale data analysis." >> application.md
	cat expectedValue.md >> application.md
	echo "\n# Landscape Analysis (" `wc -c < landscape.md` "/ 1500 words)" >> application.md
	echo "\nWe are looking for proposals from software projects with demonstrated traction and adoption. Briefly describe other software tools that the audience for this proposal primarily uses (including proprietary alternatives, if they exist), and how the software project(s) in your proposal compare in terms of user base, adoption, functionality, and maturity relative to their target audience. You can add indicators of adoption and usage as needed. Please indicate if the software is used in AI applications and workflows." >> application.md
	cat landscape.md >> application.md

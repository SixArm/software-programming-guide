top = $(shell git rev-parse --show-toplevel)
key = $(shell basename ${top})

links="tmp/links.md"
bound="tmp/bound.md"
output="tmp/${key}.pdf"
pandoc="pandoc-from-markdown-to-pdf"

all: ${links} ${bound} ${output}

new: clean all

.PHONY: clean
clean:
	rm -f ${links} ${bound} ${output}

${links}:
	sed -n '/^## Contents$$/,$$p' "${top}/README.md" | sed 's/(topics/(/' > ${links}

${bound}:
	book-binder start.yml ${links} ${bound} "${top}/topics"

${output}:
	${pandoc} ${bound} -o ${output}

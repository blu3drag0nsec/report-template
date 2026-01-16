# Report Template

> Inspired in the work of `https://github.com/noraj/OSCP-Exam-Report-Template-Markdown`


```bash
# Generate the docker image with
./build.sh
```

```bash
# Enter the container that has all the LaTeX dependencies
./run.sh
```

```bash
# Generate pdf with
./build_pdf.sh
```

## customize

> `build_pdf.sh` contains the paths from the source and the target, do not change the main folder `src` as this is hardcoded in the `osert.rb`, but you can change the report.md to something else.

> Same for `output` folder (do not change it), but you can change the filename to something else.

```sh
#!/bin/bash
ruby osert.rb generate 'src/report.md' 'output/report.pdf'
```

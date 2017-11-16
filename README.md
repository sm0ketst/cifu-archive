# cifu-archive
Python script to make a local mirror of Cifu's jazz radio shows.

### Introduction
The majority of Juan Claudio Cifuentes' body of work in advocating for Jazz in Spain is currently available in RTVE's Alacarta streaming service. All rights remain reserved to RTVE:

* http://www.rtve.es/alacarta/audios/jazz-porque-si/
* http://www.rtve.es/alacarta/audios/a-todo-jazz/

Should Alacarta ever stop offering such podcasts, this script ensures that his work is persisted and freely available for all Jazz lovers, forever. It will need around 150GB of available disk space.

It will synthesise filenames using a combination of radio show name, date (when available) and title (preserving UTF-8 character encoding). The script will by default spawn 8 worker threads to download shows in parallel.

### Caveats
* For the sake of simplicity, the cleanup of temporary files (*.tmp) must be performed manually.
* The script is idempotent in that it will not download files already on disk based on their filenames, no checksumming is performed
* The script is not flushing podcasts to disk in chunks, it'll fit it all in RAM

### Acknowledgments
* Juan Claudio "Cifu" Cifuentes (Paris, 1941 - Madrid, 2015). Love and respect. Rest in Peace.

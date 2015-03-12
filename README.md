# Google docs Onebox for Discourse

This plugin allows to embed any published document, spreadsheet, forms, and/or Presentation from Google Drive.

## Installation

As seen in a [how-to on meta.discourse.org](https://meta.discourse.org/t/advanced-troubleshooting-with-docker/15927#Example:%20Install%20a%20plugin), simply **add the plugin's repo url to your container's app.yml file**:

```yml
hooks:
  after_code:
    - exec:
        cd: $home/plugins
        cmd:
          - mkdir -p plugins
          - git clone https://github.com/discourse/docker_manager.git
          - git clone https://github.com/naveed-ahmad/google_docs_onebox.git
```
* Rebuild the container

```
cd /var/docker
git pull
./launcher rebuild app
```

## Screenshots
Spreadsheet
![Spreadsheet](https://raw.githubusercontent.com/naveed-ahmad/google_docs_onebox/screenshots/screenshots/Selection_004.png)

Presentation
![Presentation](https://raw.githubusercontent.com/naveed-ahmad/google_docs_onebox/screenshots/screenshots/Selection_005.png)

Forms
![Google Form](https://raw.githubusercontent.com/naveed-ahmad/google_docs_onebox/screenshots/screenshots/Selection_007.png)

Document
![Google document](https://raw.githubusercontent.com/naveed-ahmad/google_docs_onebox/screenshots/screenshots/Selection_006.png)


## Troublshooting 
- Make sure document,spreadsheet and presentation is published. You can puslish by clicking on "File => Publish" menu
- Copy the URL from address bar and past in discourse editor

## Contributing
Contributions are welcome. Report issue, even better send pull if you find any bug :)




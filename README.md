# Django Project Template [![Build Status](https://secure.travis-ci.org/cirlabs/django-project-template.png?branch=master)](http://travis-ci.org/cirlabs/django-project-template)

## Requirements
- [Django 1.7+](https://www.djangoproject.com/)
- [Postgres 9.3+](http://www.postgresql.org/)
- [PostGIS 2.1+](http://postgis.net/)
- [virtualenvwrapper](http://virtualenvwrapper.readthedocs.org/en/latest/)

## Quickstart
```bash
$ mkvirtualenv project_name
$ pip install django fabric
$ django-admin.py startproject --extension=py,.gitignore --template=https://github.com/cirlabs/django-project-template/archive/master.zip project_name
$ cd project_name
$ fab bootstrap
```

Need a frontend scaffold too? See [cirlabs/generator-newsapp](http://github.com/cirlabs/generator-newsapp).


## Postgis
By default, this project assumes you'll be using PostGIS as your database. If you'd prefer not to, you can set the `USE_POSTGIS` variable in `settings/common.py` to false and the project will default to PostgreSQL.

## Notes
- If you're creating a GeoDjango application on Heroku, you're going to need geo spatial libraries like GDAL and PostGIS. Luckily, CIR is here to help. Read more about our GeoDjango buildpack here: [cirlabs/heroku-buildpack-geodjango](https://github.com/cirlabs/heroku-buildpack-geodjango)

## Help
Need help? Send a pull request or open an issue in. [ISSUES](https://github.com/cirlabs/django-project-template/issues)

## Contributing
Want to improve the template? Start a new project with the master branch template and add your features/edits. Once you're done, fork the repo, add your changes and send a pull request.

## License

The MIT License (MIT)

Copyright (c) '93 Til ... The Center for Investigative Reporting

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR I

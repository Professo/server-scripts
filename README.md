# server-scripts
Various scripts for debian based shared hosting server.

## Requirements
- [drupal-scripts](https://github.com/popstas/drupal-scripts)
- [drall](https://github.com/popstas/drall)



# get-sites - ������ ������ �� ��������, ������, email ������
- ���� ��� "root" � `/etc/nginx/sites-enabled`
- ��� ������� `root` ������� ������ ����� (`server_name`)
- ���������� ������ ����� (drupal / joomla / wordpress / unknown / none)
- ��� Drupal ������� email �� `site_mail`
- ��� Joomla ������� email �� `configuration.php`
- ���� � ����� ����� ���� � ����� (�� ��������� `.info`, ������������ � `SITE_INFO_FILE`), ������� �� ���� email=*

## �������������
������, ����������� ������:  
```get-sites > /root/log/sites.log```

csv ����:  
```echo "root_path;engine;domain;email" > /root/log/sites.csv && get-sites | tr -s"\t" ";" >> /root/log/sites.csv```



# TODO:
- ��������� ������������ �� ������ ��������

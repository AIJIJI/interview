# Base

## 简单

1. 什么是 MVC 

    Models: It describes your database schema and your data structure

    Views: It controls what a user sees, the view retrieves data from appropriate models and execute any calculation made to the data

    Controller: The Django framework and URL parsing

2. 怎使用外键连接到其他应用的 model

    INSTALLED_APP

    other_app.model_cls


# REST Framework

1. Serializer 有哪些确定 fields 的方式

    fields, exclude

2. Serializer 的 partial  /'pɑrʃəl/ 参数 有什么用

    By default, serializers must be passed values for all required fields or they will raise validation errors. You can use the partial argument in order to allow partial updates.

3. ViewSet 的 filter_backends 字段是做什么的

    A list of filter backend classes that should be used for filtering the queryset. Defaults to the same value as the DEFAULT_FILTER_BACKENDS setting.
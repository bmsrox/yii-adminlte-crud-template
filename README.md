YII ADMINLTE CRUD TEMPLATE
==========================

This is a code template to adminlte integrated with yii2

    composer require bmsrox/yii-adminlte-crud-template

or add into composer.json

    "bmsrox/yii-adminlte-crud-template": "dev-master"
    
## CONFIG GII LAYOUT

Into your backend/config/main-local.php edit the follow instruction:

```````
$config['modules']['gii'] = [
        'class' => 'yii\gii\Module',
          'generators' => [ //here
            'crud' => [ // generator name
                'class' => 'yii\gii\generators\crud\Generator', // generator class
                'templates' => [ //setting for out templates
                    'custom' => '@vendor/bmsrox/yii-adminlte-crud-template', // template name => path to template
                ]
            ]
        ],
    ];
```````

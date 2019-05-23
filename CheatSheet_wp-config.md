# Liste d'options Wordpress utile

## Debug
define( 'WP_DEBUG', true );

## Configuration générale
### Site URL 
```
define( 'WP_HOME', 'https://url/' );
define( 'WP_SITEURL', 'https://url/' );
```

## Performance
### Désactiver les crons http 
Pensez à faire un cron systeme avec un wget sur https://url/wp-cron.php?doing_wp_cron
```
define('DISABLE_WP_CRON', true);
```

### Activer le cache + url du plugin
```
define('WP_CACHE', true);
define('WPCACHEHOME','/$WebRootFolder/wp-content/plugins/wp-super-cache/');
```

### Autoriser le telechargement direct de plugins/themes via le backend ..
```
define( 'FS_METHOD', 'direct' );
```

### Interdire la modification de fichier via le backend
```
define( 'DISALLOW_FILE_EDIT', 'true' );
```

### Augmenter la mémoire dédié à Wordpress 
```
define('WP_MEMORY_LIMIT', '256M');
```

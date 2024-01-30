# A Platform That Forgives Your Mistakes

Have you deleted critical content from your site, or made some code changes that broke something? Don't worry, it happens to the best of us. Fortunately, WordPress.com's backup and restore features make it easy to recover your site.

## Real-Time Backups

The Real-Time Backups feature is a safety net for your site. Backups are created at least once a day, or even multiple backups per day when multiple changes are detected. Backups cover all essential components of your website:

- Pages, posts, media files, and other `wp-content` folder contents
- Installed themes and plugins
- Root-level WordPress files
- WordPress database. Specifically, any tables that begin with your WordPress table prefix and have a unique or primary key.

However, it's important to note that some elements are not backed up:

- Core WordPress files
- Files outside specific directories
- Database tables that don’t look like they belong to WordPress or whose rows have no unique identifier.
- Cache and backup directories

## Accessing and Managing Your Backups

You can see the backups of your site, and restore to a previous backup, from your site's dashboard. To access your backups:

1. Go to your site's dashboard.
2. Hover over Jetpack and select Backup.
3. Navigate to the desired backup using the on-screen options.

Note that restores can take varying amounts of time, depending on the size and complexity of your site.

## Conclusion

With WordPress.com's backup and restore capabilities, you have the power to easily correct mistakes and maintain the integrity of your website. It's a platform that not only hosts your digital presence but also protects and forgives the inevitable errors in website management.

For more detailed information and assistance, visit [WordPress.com Support](https://wordpress.com/support/restore/).

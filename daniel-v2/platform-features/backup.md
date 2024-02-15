# Real Time Backup

**VaultPress Backup** by Jetpack automatically saves every change and helps you get back online quickly with one‑click restores. This guide will show you how to access your site’s backups and restore your website to any previous point in time.

This feature is available on sites with the [WordPress.com Creator or Entrepreneur plan](https://wordpress.com/plans/). If your site has one of our legacy plans, it is available on the Pro plan.

## About Backups

**VaultPress Backup** is included in [eligible plans](https://wordpress.com/plans/) and backs up your site automatically. As a site owner, you don’t need to worry about backing up your site manually or installing extra plugins — we take care of it for you.

Backups are saved at least once per day, typically 24 hours after the previous backup. Backups can also occur multiple times in a single day if many changes are being made to the site.

We back up the following data:

- Your pages, posts, media files, followers, and other content in your `wp-content` folder.
- Your installed themes and plugins.
- Your site’s root-level WordPress files.
- Your site’s WordPress database. Specifically, any tables that begin with your WordPress table prefix and have a unique or primary key.

The following data is not backed up:

- The core files of WordPress, which are managed for you by WordPress.com.
- Files outside the directories listed above.
- Database tables that don’t look like they belong to WordPress or whose rows have no unique identifier.
- Cache and backup directories.
- Additional WordPress installs, such as ones that are included inside a subdirectory.

Backups are retained for as long as your site has an eligible [plan](https://wordpress.com/plans/). If your plan [expires](https://wordpress.com/support/restore-your-site-after-the-plan-expires/), backups are kept for 30 days after expiry.

## Access Your Backups

To view your backups, follow these steps:

1.  Visit your site’s [dashboard](https://wordpress.com/home).
2.  On the left side, hover your mouse over *Jetpack*.
3.  Select **Backup**.

This will display the most recent backup. Using the navigation options at the top of the screen, you can navigate to any previous backups from the past.

The same backups can be found in your site’s** [Activity](https://developer.wordpress.com/docs/troubleshooting/activity-log/)** at *Jetpack → [Activity Log](https://wordpress.com/activity-log/)*.

<figure class="wp-block-image size-full">![the WordPress Jetpack menu with Backup highlighted](https://wpdeveloperstaging.files.wordpress.com/2024/02/jetpack-backup.png)</figure>

Click on the **Actions** button in the top right corner of a backup:

<figure class="wp-block-image size-full">![Panel displaying the available actions for the selected Jetpack Backup](https://wpdeveloperstaging.files.wordpress.com/2024/02/backup-restore-jetpack.png)</figure>

Here, you will find the following options:

- **Restore to this point**: This option will [restore your site](https://wordpress.com/support/restore/#restore-from-a-backup) to the backup created on the date selected. This option will also display under the backup date and time.
- **View files**: This option will provide access to the selected backup files. You can navigate and choose individual files, plugins, themes, or database tables and download them directly to your local storage.
- **Download backup**: This option downloads a copy of your site to your computer to use on a self-hosted WordPress site or local install. Downloaded backups cannot be used to restore your site on WordPress.com, so choose the “**Restore to this point**” button for this purpose.

## When to Use Backups

Backups are a great tool to use if:

- You are missing content or wish to undo a change that cannot be restored via [post and page revisions](https://wordpress.com/support/editors/page-post-revisions/).
- You wish to reset your site to a previous point in time (up to six months ago.)
- You’ve installed a plugin/theme that breaks your site, a backup is available to you, and you know for sure which plugin/theme is responsible.
  - To determine which plugin is causing an error on your site, follow the steps in the [Solve Problems With Plugins](https://wordpress.com/support/plugins/solve-problems-with-plugins/) guide.

## Restore From a Backup

Restoring a backup returns your site to exactly how it was at that point in time. Therefore, any changes you made after that point in time may be lost. If you wish to preserve any content created after your restore point, [see this section](#retain-after-restore).

To restore your WordPress.com site to a previous point in time:

1.  Visit your site’s [dashboard](https://wordpress.com/home).
2.  On the left side, go to *Jetpack → Backup* or *Jetpack → Activity Log*.
3.  Navigate back to the date and time of the backup you wish to restore.
4.  Click the **Restore** button:

<figure class="wp-block-image size-full is-resized">![An arrow points to a button that says restore to this point](https://wpdeveloperstaging.files.wordpress.com/2024/02/jetpack-backup-restore.png)</figure>

<figure class="wp-block-image size-full">![An arrow points to a button that says restore](https://wpdeveloperstaging.files.wordpress.com/2024/02/jetpack-activity-restore.png)</figure>

1.  You’ll then be asked to confirm which parts of the site you’d like to restore. Leave all boxes checked to restore every part of your site to your chosen backup time. Alternatively, you can tick or untick the boxes for the following parts of your site:

- **WordPress themes:** This will restore your site’s theme folder to what it was at that point in time. Depending on your third-party theme, this will not necessarily restore a theme’s settings when those settings are saved outside of the theme folder.
- **WordPress plugins: **This will restore your site’s plugin folder to what it was at that point in time. Depending on the third-party plugin you are using, this will not necessarily restore a plugin’s settings that may be saved outside of this folder.
- **WordPress root**: This will restore WordPress root files related to your site’s configuration, including wp-config.php and any non-WordPress files.
- **WP-content directory**: This will restore the wp-content folder and its contents to the state it was in at the time of the backup. Please note that this will not restore the themes, plugins, or media uploads folders, which you can include or exclude separately.
- **Site database**: This will restore content for posts, pages, comments, and (depending on the third-party themes and plugins) some plugin and theme settings.
- **Media uploads: **This will restore the contents of your [media library](https://wordpress.com/support/media/) to what was in there at that point in time. You must also select ‘_Site database_‘ for restored media uploads to appear.

1.  Click the “**Confirm restore**” button to begin restoring your site. Once it has completed, you’ll receive an email notification.

<figure class="wp-block-image size-full">![A Jetpack VaultPress backup just starting, with the progress at 0%](https://wpdeveloperstaging.files.wordpress.com/2024/02/jetpack-backup-started.png)</figure>

Please note that backups may take some time to complete, which can range from a few minutes to a few hours, depending on the size of your site. You can safely navigate away from the screen while the restore is in progress.

<figure class="wp-block-image size-full">![Panel displaying the available actions for the selected Jetpack Backup](https://wpdeveloperstaging.files.wordpress.com/2024/02/jetpack-backup-complete.png)</figure>

### Retain Content Created After Restore Point

You may need to restore a backup but preserve some content you added or modified after your chosen restore point. Before you begin [restoring your site,](https://wordpress.com/support/restore/#restore-from-a-backup) make a copy of the content.

If it’s a small amount of changes, such as the text of a blog post, copy and paste it into another program on your computer. You can then add it back to your site after the backup has finished restoring.

For large changes to your site’s content, [export your site’s content](https://wordpress.com/support/export/).

If your changes include *Media* (such as images or video uploads), you must import the content into another WordPress site – you can [create a free site in your account](https://wordpress.com/support/create-multiple-websites/) for this purpose. This is because export files do not store media files. They only contain links to media files, which are then uploaded upon importing to another WordPress site.

When you’ve completed the restore on your original site, export the content from the free site and import it into your original site. Doing so will update just the pages and posts that need to be updated, leaving your plugins and other configurations in place.

## Frequently Asked Questions

**What will happen to my WooCommerce orders if I restore a backup?**

We’ve developed Jetpack VaultPress Backup with WooCommerce in mind. You can safely restore your site to any past state — all orders and products will be kept current.

**I have a `.tar.gz` file from my previous backup, and I want to restore it. How do I do that?**

The `.tar.gz` backup file needs to be restored manually. To do so, follow the guide to [Manually Restore a Backup](https://jetpack.com/support/manually-restore-a-backup/), starting from step 5.

**I want to migrate one WordPress.com site to another WordPress.com site. Can I do that with a Jetpack Backup?**

This is possible but can be a challenging process. The recommended method for this type of migration is either to:

- [Export the content from the source site to XML](https://wordpress.com/support/export/#export-content-to-another-word-press-site) via *Tools → Export*, and then import to the destination site
- Use a plugin such as [All in One WP Migration](https://wordpress.com/support/import/import-using-all-in-one-migration/) to create an export of your source site and then import that content to the destination site.

**How do I exclude certain files from being backed up?**

You have two options for excluding certain files from being backed up:

- **Create a new directory to exclude:** You can move files to a new directory called `donotbackup`. Jetpack VaultPress Backup will know to skip this directory automatically. This is a great way to reduce the storage size of your backups.
- **Exclude an existing directory:** You can add a file called `.donotbackup` to any existing directory. Jetpack VaultPress Backup will skip the entire directory that includes the `.donotbackup` file.

[](https://wordpress.com/support/restore/#retain-content-created-after-restore-point)

[](https://wordpress.com/support/restore/#restore-from-a-backup)

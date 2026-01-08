# Varbase Admin Base

A recipe to manage default installed modules, configs and permissions for Varbase admin experience.

This recipe provides a complete admin setup including:
- Admin audit trail modules for comprehensive activity logging
- Masquerade for testing user experiences
- Menu administration per menu
- Responsive preview for testing responsive designs
- Revision log defaults for better content tracking
- Autosave form for preventing content loss
- Entity clone for duplicating content
- Taxonomy manager and taxonomy access fix
- Coffee for quick administration navigation
- Length indicator for fields
- Navigation module with extra tools
- Gin admin theme with toolbar, login, and everywhere integrations
- Trash module for soft delete functionality
- ECA VBO for bulk operations workflows

## Features

### Admin Experience
- **Gin Admin Theme**: Modern, accessible admin interface with toolbar, login page, and everywhere integration
- **Navigation Module**: Enhanced navigation with extra tools, cache flushing, and cron access
- **Coffee**: Quick administration menu for fast navigation
- **Responsive Preview**: Test your site's appearance on various devices (iPhone 15, Galaxy S23, iPad Pro, etc.)

### Content Management
- **Entity Clone**: Duplicate nodes, blocks, taxonomy terms, and more
- **Autosave Form**: Automatic draft saving to prevent content loss
- **Revision Log Default**: Better revision tracking
- **Length Indicator**: Visual feedback on field length limits
- **Trash**: Soft delete functionality with auto-purge options

### User Management & Security
- **Masquerade**: Test the site as different users
- **Menu Admin Per Menu**: Granular menu permissions
- **Admin Audit Trail**: Comprehensive activity logging for files, media, users, taxonomy, nodes, menus, and authentication

### Taxonomy & Organization
- **Taxonomy Manager**: Enhanced taxonomy term management
- **Taxonomy Access Fix**: Proper taxonomy access controls

### Automation
- **ECA VBO**: Event-Condition-Action integration with Views Bulk Operations

## Permissions

The recipe configures permissions for the following roles:
- **Authenticated**: Basic shortcut access and user profile editing
- **Editor**: Content creation and management permissions
- **SEO Admin**: SEO-related permissions
- **Content Admin**: Advanced content management permissions
- **Site Admin**: Full administrative permissions including masquerading, user management, and menu administration

Add the recipe using composer:
```
composer require drupal/varbase_admin_base:~1.0.0
```

Change directory to `/web` or `/docroot`

Run the Drupal recipe bash script:
```
bash core/scripts/drupal recipe recipes/contrib/varbase_admin_base
```

or

Run the Drush recipe command:
```
drush recipe recipes/contrib/varbase_admin_base
```

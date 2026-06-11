# Architecture Summary

This document provides a high-level architectural overview only. It intentionally
omits implementation details, database schemas, source paths, and deployment
configuration.

## Backend

The private application uses Laravel as the core backend framework. It manages
authentication, administrative workflows, content entities, media records,
settings, backups, and public page delivery.

## Admin Interface

The administrative experience is implemented as a modern single-page workflow
using Vue and Inertia. This keeps editorial actions responsive while preserving
Laravel as the application authority.

## Public Interface

The public website is rendered through server-side templates with lightweight
client-side interaction where needed. This approach supports SEO-friendly pages
and predictable frontend performance.

## Data Layer

Content, media metadata, navigation, user roles, advertisements, settings, and
operational records are stored in a relational database. The public repository
does not include migrations, seeders, dumps, or schema files.

## Deployment

Deployment assets and environment-specific configuration are private. This public
repository is not sufficient to build, deploy, or run Serapan CMS.

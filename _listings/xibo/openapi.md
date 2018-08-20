---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /playlist/widget/ticker/{playlistId}:
    post:
      summary: Add a ticker Widget
      description: Add a new ticker Widget to the specified playlist
      operationId: WidgetTickerAdd
      x-api-path-slug: playlistwidgettickerplaylistid-post
      parameters:
      - in: formData
        name: allowedAttributes
        description: EDIT Only and SourceId=1 - A comma separated list of attributes
          that should not be stripped from the feed
      - in: formData
        name: backgroundColor
        description: Edit only - A HEX color to use as the background color of this
          widget
      - in: formData
        name: copyright
        description: EDIT Only and SourceId=1 - Copyright information to display as
          the last item in this feed
      - in: formData
        name: css
        description: Optional StyleSheet Pass only with overrideTemplate set to 1
          or with sourceId=2
      - in: formData
        name: dataSetId
        description: For sourceId=2, Create ticker Widget using provided dataSetId
          of an existing dataSet
      - in: formData
        name: dateFormat
        description: EDIT Only - The date format to apply to all dates returned by
          the ticker
      - in: formData
        name: disableDateSort
        description: EDIT Only, SourceId=1 - Should the date sort applied to the feed
          be disabled?
      - in: formData
        name: duration
        description: The Widget Duration
      - in: formData
        name: durationIsPerItem
        description: A flag (0, 1), The duration specified is per item, otherwise
          it is per feed
      - in: formData
        name: effect
        description: 'Edit only - Effect that will be used to transitions between
          items, available options: fade, fadeout, scrollVert, scollHorz, flipVert,
          flipHorz, shuffle, tileSlide, tileBlind, marqueeUp, marqueeDown, marqueeRight,
          marqueeLeft'
      - in: formData
        name: filter
        description: EDIT Only, SourceId=2 - SQL clause for filter this dataSet
      - in: formData
        name: itemsPerPage
        description: EDIT Only - When in single mode, how many items per page should
          be shown
      - in: formData
        name: itemsSideBySide
        description: A flag (0, 1), Should items be shown side by side
      - in: formData
        name: javaScript
        description: Optional JavaScript, Pass only with overrideTemplate set to 1
      - in: formData
        name: lowerLimit
        description: EDIT Only, SourceId=2 - Lower low limit for this dataSet, 0 for
          nor limit
      - in: formData
        name: name
        description: Optional Widget Name
      - in: formData
        name: noDataMessage
        description: EDIT Only - A message to display when no data is returned from
          the source
      - in: formData
        name: numItems
        description: EDIT Only and SourceId=1 - The number of RSS items you want to
          display
      - in: formData
        name: ordering
        description: EDIT Only, SourceId=2- SQL clause for how this dataSet should
          be ordered
      - in: formData
        name: overrideTemplate
        description: EDIT Only, SourceId=1 - flag (0, 1) override template checkbox
      - in: path
        name: playlistId
        description: The playlist ID to add a Widget to
      - in: formData
        name: randomiseItems
        description: A flag (0, 1), whether to randomise the feed
      - in: formData
        name: sourceId
        description: Add only - 1 for rss feed, 2 for dataset
      - in: formData
        name: speed
        description: Edit only - The transition speed of the selected effect in milliseconds
          (1000 = normal) or the Marquee speed in a low to high scale (normal = 1)
      - in: formData
        name: stripTags
        description: EDIT Only and SourceId=1 - A comma separated list of attributes
          that should be stripped from the feed
      - in: formData
        name: takeItemsFrom
        description: 'EDIT Only and SourceId=1 - Take the items form the beginning
          or the end of the list, available options: start, end'
      - in: formData
        name: template
        description: Template for each item, replaces [itemsTemplate] in main template,
          Pass only with overrideTemplate set to 1 or with sourceId=2
      - in: formData
        name: templateId
        description: 'EDIT Only, SourceId=1 - Template youd like to apply, options
          available: title-only, prominent-title-with-desc-and-name-separator, media-rss-with-title,
          media-rss-wth-left-hand-text, media-rss-image-only'
      - in: formData
        name: textDirection
        description: 'EDIT Only, SourceId=1 - Which direction does the text in the
          feed use? Available options: ltr, rtl'
      - in: formData
        name: updateInterval
        description: EDIT Only - Update interval in minutes
      - in: formData
        name: upperLimit
        description: EDIT Only, SourceId=2 - Upper low limit for this dataSet, 0 for
          nor limit
      - in: formData
        name: uri
        description: For sourceId=1, the link for the rss feed
      - in: formData
        name: useDuration
        description: (0, 1) Select 1 only if you will provide duration parameter as
          well
      - in: formData
        name: useFilteringClause
        description: EDIT Only, SourceId=2 - flag (0,1) Use advanced filter clause
          - set to 1 if filter is provided
      - in: formData
        name: useOrderingClause
        description: EDIT Only, SourceId=2 - flag (0,1) Use advanced order clause
          - set to 1 if ordering is provided
      responses:
        200:
          description: OK
      tags:
      - Ticker
      - Widget
---
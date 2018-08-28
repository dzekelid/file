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
  /playlist/widget/{widgetId}/audio:
    put:
      summary: Parameters for edting/adding audio file to a specific widget
      description: Parameters for edting/adding audio file to a specific widget
      operationId: WidgetAssignedAudioEdit
      x-api-path-slug: playlistwidgetwidgetidaudio-put
      parameters:
      - in: formData
        name: loop
        description: Flag (0, 1) Should the audio loop if it finishes before the widget
          has finished?
      - in: formData
        name: mediaId
        description: Id of a audio file in CMS library you wish to add to a widget
      - in: formData
        name: volume
        description: Volume percentage(0-100) for this audio to play at
      - in: path
        name: widgetId
        description: Id of a widget to which you want to add audio or edit existing
          audio
      responses:
        200:
          description: OK
      tags:
      - Parametersedting
      - Adding
      - Audio
      - File
      - To
      - Specific
      - Widget
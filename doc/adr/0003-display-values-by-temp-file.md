# 3. Display values by temp file

Date: 2025-03-21

## Status

Accepted

## Context

The oled display need data source to provide values from measurments. InfluxDB can wait long after start with providing those values so we will workaround it with 

## Decision

There will be shared folder in pat /app/display/ with files Up.txt and down.txt - each odf them takes two lines of display. Lines can contain aprox 20 chars (depends from font)

## Consequences

It is stupid but it is working so good enough :)
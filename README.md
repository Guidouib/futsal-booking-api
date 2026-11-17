# Futsal Booking API

REST API for booking and prepaying futsal matches, built with .NET 10.

## Context

A WhatsApp group of ~1,000 players organizes weekly futsal matches.
Spots are limited and often oversubscribed, so bookings are handled
manually and payments are hard to track. This API replaces that process.

## Features

- Create matches with limited capacity and price per player
- Book and cancel spots
- Waitlist: when a booking is cancelled, the first player in line gets the spot
- Cancellation deadline: no refund within 2 hours of kickoff
- Commission calculation per booking

## Tech stack

- .NET 10 (LTS) — Minimal APIs
- Entity Framework Core
- SQL Server

## Running locally

    dotnet run --project src/FutsalBooking.Api

The OpenAPI document is served at `/openapi/v1.json`.

## Status

In development.

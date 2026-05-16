# Cosmo

A real-time PostgreSQL internals dashboard for your terminal.
Built in Go using Bubbletea and Lipgloss.

## What is Cosmo?

Cosmo gives you a live view into your PostgreSQL database 
internals directly from the terminal. No browser, no 
external tools — just your database and your terminal.

## Dashboard Panels

**DB Overview** — database size, active connections, 
cache hit ratio, server uptime

**Active Queries** — live view of running queries, 
their state and duration

**WAL & MVCC** — current WAL LSN, dead tuples, 
live tuples, checkpoint count

**Locks & Waits** — active locks and blocked queries

Auto-refreshes every 2 seconds.

## Setup

**Requirements**
- PostgreSQL 17+
- Go 1.26+

**Clone**

`git clone https://github.com/mujib77/cosmo`

`cd cosmo`

**Create .env**
`DATABASE_URL=postgres://user:password@localhost:5432/dbname`

**Run**

`go run main.go`

## Built With

- Go
- Bubbletea — TUI framework
- Lipgloss — terminal styling
- pgx — PostgreSQL driver
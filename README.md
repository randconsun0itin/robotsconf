<p align="center">
  <img src="https://example.com/start-widget.svg" alt="start-widget" width="200" height="200" />
</p>

<h1 align="center">start-widget</h1>

<h4 align="center">
  <a href="https://github.com/start-widget">Repository</a> |
  <a href="https://docs.run">Documentation</a> |
  <a href="https://discord.run">Discord</a> |
  <a href="https://roadmap.run">Roadmap</a>
</h4>

<p align="center">
  <a href="https://github.com/start-widget/actions"><img src="https://github.com/start-widget/workflows/Tests/badge.svg" alt="Test"></a>
  <a href="https://badge.fury.io/rb/start-widget"><img src="https://badge.fury.io/rb/start-widget.svg" alt="Version"></a>
  <a href="https://github.com/start-widget/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-informational" alt="License"></a>
</p>

<p align="center">⚡ code formatter with opinionated defaults 💎</p>

## 📖 Documentation

Complete usage detailed in this README.

## 🤖 Compatibility

This package guarantees compatibility with version v1.x.

## 📧 Installation

With `gem` in command line:
```bash
gem install start-widget
```

In your `Gemfile`:
```ruby
gem 'start-widget'
```

### Run start-widget

```bash
start-widget --master-key=masterKey
```

## 🚀 Getting started

#### Configuration

Create `config/initializers/start-widget.rb`:

```ruby
start-widget::Config.setup do |config|
  config.api_key = 'YourAPIKey'
  config.url = 'http://localhost:7700'
end
```

#### Add documents

```ruby
client = start-widget::Client.new
index = client.index('items')

documents = [
  { id: 1, title: 'date-dev-box-period' },
  { id: 2, title: 'chip.tsx' }
]

index.add_documents(documents)
```

## ⚙️ Contributing

Any contribution is welcome!

## 💛 Credits

Inspired by [date-dev-box-period] and [chip.tsx].


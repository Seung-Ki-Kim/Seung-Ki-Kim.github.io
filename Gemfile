# frozen_string_literal: true

source "https://rubygems.org"

# 시스템에 필요한 기본 라이브러리
gem "json"
gem "rake" # <--- protobuf 빌드 에러 방지를 위해 명시적으로 추가합니다.

# Chirpy 테마 의존성
gem "sass-embedded", "~> 1.70.0"

gemspec

group :test do
  gem "html-proofer", "~> 5.0"
end

# 플랫폼별 설정 최적화
# 리눅스(GitHub Actions)에서도 tzinfo가 필요할 수 있으므로 범위를 넓힙니다.
gem "tzinfo", ">= 1", "< 3"

platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo-data"
end

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-include-cache"
  gem "jekyll-paginate"
  gem "jekyll-archives"
  gem "jekyll-seo-tag"
  gem "jekyll-gist"
  gem "jemoji"
  gem "jekyll-sitemap"
end

# wdm은 윈도우 전용이므로 플랫폼 제약을 확실히 둡니다.
gem "wdm", "~> 0.2.0", platforms: [:mingw, :x64_mingw, :mswin]

gem "jekyll"
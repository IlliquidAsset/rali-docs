# RALI Code Index

## **1. Custom Classes & State Management**
- **`state/navigation/navigation_controller.dart`** - Manages navigation state.
  - **Class:** `NavigationController`
  - **Variables:** `currentRoute`, `destination`, `isNavigating`, `isRerouting`, `mode`, `progress`
  - **Methods:** `planRoute()`, `setMode()`, `startNavigation()`, `stopNavigation()`, `updateLocation()`

- **`state/navigation/navigation_types.dart`** - Defines core navigation types and modes.
  - **Enums:** `RouteEmphasis`, `RALINavigationMode`

- **`state/navigation/navigation_state.dart`** - Tracks navigation status.
  - **Class:** `RALINavigationState`
  - **Variables:** `status`, `progress`, `remainingDistance`, `mode`, `isNavigating`, `destination`
  - **Methods:** `copyWith()`

- **`state/weather/weather_state.dart`** - Manages weather state.
  - **Class:** `WeatherState`
  - **Variables:** `currentWeather`, `isLoading`, `errorMessage`
  - **Methods:** `fetchWeather()`

- **`state/search/search_state.dart`** - Manages search bar state.
  - **Class:** `SearchState`
  - **Variables:** `query`, `results`, `isSearching`
  - **Methods:** `clearSearch()`, `startSearching()`, `updateResults()`

- **`state/search/search_controller.dart`** - Handles search logic.
  - **Class:** `SearchController`
  - **Methods:** `performSearch()`

- **`state/weather/weather_controller.dart`** - Manages weather overlays.
  - **Class:** `WeatherController`
  - **Variables:** `weatherApi`, `weatherState`
  - **Methods:** `updateWeather()`

## **2. Services & APIs**
- **`services/navigation/route_service.dart`** - Handles route calculations and Mapbox API requests.
  - **Class:** `RouteService`
  - **Methods:** `getRoute()`, `displayRoute()`, `clearRoute()`

- **`services/navigation/navigation_types.dart`** - Defines navigation-related types and enums.
  - **Enums:** `RouteEmphasis`, `RALINavigationMode`

- **`services/navigation/route_details.dart`** - Stores detailed route metadata.
  - **Class:** `RouteDetails`
  - **Variables:** `points`, `distance`, `duration`, `steps`, `bounds`
  - **Methods:** `fromMapboxRoute()`, `getEstimatedArrival()`, `getDistanceInKilometers()`

- **`services/api/weather_api.dart`** - Handles weather data retrieval.
  - **Class:** `WeatherApi`
  - **Methods:** `getCurrentPrecipitation()`, `getCurrentWeather()`, `getHourlyForecast()`

- **`services/search_service.dart`** - Implements place search functionality.
  - **Class:** `SearchService`
  - **Methods:** `searchPlaces()`, `reverseGeocode()`

## **3. Theme & UI Components**
- **`theme/rali_typography.dart`** - Defines typography styles.
  - **Class:** `RALITextTheme`
  - **Variables:** `textTheme`

- **`theme/rali_colors.dart`** - Stores color constants.
  - **Class:** `RALIColors`
  - **Variables:** `primary`, `secondary`, `error`, `success`, `background`

- **`theme/rali_animations.dart`** - Standardized animations.
  - **Class:** `RALIAnimationCurve`
  - **Variables:** `accelerate`, `decelerate`, `standard`

## **4. Widgets & Controls**
- **`widgets/control_button.dart`** - Standard button component.
  - **Class:** `ControlButton`
  - **Variables:** `child`, `isActive`, `onTap`
  - **Methods:** `build()`

- **`widgets/search_bar.dart`** - Search bar UI component.
  - **Class:** `SearchBar`
  - **Variables:** `controller`, `searchService`, `showClearButton`
  - **Methods:** `createState()`

## **5. Configuration & Utilities**
- **`config/app_config.dart`** - Loads environment configurations.
  - **Methods:** `loadEnvFromServer()`

- **`utils/map_utils.dart`** - Helper functions for Mapbox interactions.
  - **Class:** `MapUtils`
  - **Methods:** `createCameraPosition()`, `createLocationMarker()`

- **`utils/position_utils.dart`** - Provides coordinate conversions.
  - **Class:** `RaliPosition`
  - **Variables:** `lat`, `lng`
  - **Methods:** `bearingTo()`, `distanceTo()`, `toMapboxPoint()`

## **Next Steps**
- Verify all classes, variables, and methods are implemented correctly.
- Expand Dart documentation within files.
- Standardize class and function names across all modules.

2025.03.06
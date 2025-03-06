# RALI Code Index

## **1. Custom Classes & State Management**
- **`state/navigation/navigation_controller.dart`** - Manages navigation state.
- **`state/navigation/navigation_types.dart`** - Defines core navigation types and modes.
- **`state/navigation/navigation_state.dart`** - Tracks navigation status.
- **`state/navigation/ral_navigation_state.dart`** - Contains state definitions for navigation modes.
- **`state/weather/weather_state.dart`** - Manages weather state.
- **`state/search/search_state.dart`** - Manages search bar state.
- **`state/search/search_controller.dart`** - Handles search logic.
- **`state/weather/weather_controller.dart`** - Manages weather overlays.
- **`state/navigation/route_details.dart`** - Holds route details.

## **2. Services & APIs**
- **`services/navigation/route_service.dart`** - Handles route calculations.
- **`services/navigation/navigation_types.dart`** - Defines navigation-related types.
- **`services/navigation/route_details.dart`** - Stores detailed route metadata.
- **`services/api/mapbox_api.dart`** - Manages Mapbox API interactions.
- **`services/api/weather_api.dart`** - Handles weather data retrieval.
- **`services/search_service.dart`** - Implements place search functionality.
- **`services/location/location_service.dart`** - Fetches user location.

## **3. Theme & UI Components**
- **`theme/rali_typography.dart`** - Defines typography styles.
- **`theme/rali_colors.dart`** - Stores color constants.
- **`theme/rali_spacing.dart`** - Manages spacing and layout.
- **`theme/rali_elevations.dart`** - Configures elevation/shadow effects.
- **`theme/rali_theme.dart`** - Central theme management.
- **`theme/rali_animations.dart`** - Standardized animations.

## **4. Widgets & Controls**
- **`widgets/control_button.dart`** - Standard button component.
- **`widgets/control_buttons_group.dart`** - Grouped control buttons.
- **`widgets/search_bar.dart`** - Search bar UI component.
- **`widgets/navigation_overlay.dart`** - Displays navigation route overview and controls.

## **5. Configuration & Utilities**
- **`config/app_config.dart`** - Loads environment configurations.
- **`config/constants.dart`** - Stores app-wide constants.
- **`config/environment.dart`** - Manages environment settings.
- **`utils/map_utils.dart`** - Helper functions for Mapbox interactions.

## **Next Steps**
- Ensure all referenced files exist and match their expected functionality.
- Consider expanding `dartdoc` comments for more detailed documentation.
- If hosting docs, configure GitHub Pages to serve `/docs/`.
- Standardize class names across all modules for consistency.
- Verify that `RALINavigationState`, `RALINavigationMode`, and `RouteDetails` are correctly referenced and implemented.


#include <iostream>
class Point {
public:
    int x;
    int y;

    Point(int xVal, int yVal) : x(xVal), y(yVal) {}

    friend std::ostream& operator << (std::ostream& os, const Point& point) {
        os << "Point: (" << point.x << ", " << point.y << ")";
        return os;
    }
};

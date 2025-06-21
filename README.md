
import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { MapPin, PlaneTakeoff } from "lucide-react";

export default function TravelWeb// File: TravelWebsite.jsxsite() {
  return (
    <div className="bg-white min-h-screen text-gray-800 font-sans">
      <header className="bg-blue-600 text-white py-6 px-10 shadow-md">
        <h1 className="text-3xl font-bold">Hà Giang Travel 🌄</h1>
        <p className="text-sm mt-2">Khám phá vẻ đẹp hùng vĩ của miền núi phía Bắc Việt Nam</p>
      </header>

      <section className="p-10">
        <h2 className="text-2xl font-semibold mb-6">Tour nổi bật</h2>
        <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
          <Card className="hover:shadow-xl transition-all duration-300">
            <img src="https://source.unsplash.com/featured/?mountain,vietnam" alt="Tour" className="rounded-t-xl" />
            <CardContent className="p-4">
              <h3 className="text-lg font-bold">Hà Giang Loop 3N2Đ</h3>
              <p className="text-sm text-gray-600 mt-2">Trải nghiệm cung đường đèo Mã Pì Lèng, phố cổ Đồng Văn...</p>
              <Button className="mt-4 w-full" variant="outline">
                <PlaneTakeoff className="mr-2 h-4 w-4" /> Đặt tour
              </Button>
            </CardContent>
          </Card>

          <Card>
            <img src="https://source.unsplash.com/featured/?ricefield,vietnam" alt="Tour" className="rounded-t-xl" />
            <CardContent className="p-4">
              <h3 className="text-lg font-bold">Mùa lúa chín Hoàng Su Phì</h3>
              <p className="text-sm text-gray-600 mt-2">Chiêm ngưỡng ruộng bậc thang vàng óng vào mùa thu.</p>
              <Button className="mt-4 w-full" variant="outline">
                <MapPin className="mr-2 h-4 w-4" /> Xem chi tiết
              </Button>
            </CardContent>
          </Card>

          <Card>
            <img src="https://source.unsplash.com/featured/?village,vietnam" alt="Tour" className="rounded-t-xl" />
            <CardContent className="p-4">
              <h3 className="text-lg font-bold">Văn hóa bản làng</h3>
              <p className="text-sm text-gray-600 mt-2">Giao lưu với người dân tộc, thưởng thức ẩm thực địa phương.</p>
              <Button className="mt-4 w-full" variant="outline">
                <MapPin className="mr-2 h-4 w-4" /> Xem chi tiết
              </Button>
            </CardContent>
          </Card>
        </div>
      </section>

      <footer className="bg-gray-100 text-center py-6 text-sm text-gray-500">
        © 2025 Hà Giang Travel. All rights reserved.
      </footer>
    </div>
  );
}
